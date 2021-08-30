<template>
  <form @submit.prevent="submitData" >
    <div>
      <label>Name</label>
      <input type="text" v-model="enteredName" />
    </div>
    <div>
      <label>Phone</label>
      <input type="tel" v-model="enteredEmail" />
    </div>
    <div>
      <label>E-Mail</label>
      <input type="email" v-model="eneredEmail" />
    </div>
    <div>
      <button>Add Contact</button>
    </div>
  </form>
</template>

<script>
export default {
  emits: ['add-contact'],
  data() {
    return {
      enteredName: '',
      enteredPhone: '',
      enteredEmail: '',
    };
  },
  method: {
    submitData() {
      this.$emit(
        'add-contact',
        this.enteredName,
        this.enteredPhone,
        this.enteredEmail,
      );
    },
  },
};
</script>
