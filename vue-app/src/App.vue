<template>
  <section>
    <header>
      <h2>My Friends</h2>
    </header>
    <ul>
      <friend-contact
        name="Jeff Ripke"
        phone-number="333-323-3332"
        email-address="hhhhhd@djhkhk.com"
        is-favorite="1"
      ></friend-contact>
      <friend-contact
        name="Hailey Ripke"
        phone-number="333-332-3332"
        email-address="dfdsd@djhkhk.com"
        is-favorite="0"
      ></friend-contact>
    </ul>
  </section>
</template>

<script>
import FriendContact from './components/FriendContact.vue';

export default {
  components: { FriendContact },
  data() {
    return {
      friends: [
        {
          id: 'Max',
          name: 'Maximillion',
          email: 'fict@email.com',
        },
        {
          id: 'Jeff',
          name: 'Maximillion',
          email: 'fict@email.com',
        },
      ],
    };
  },
};
</script>

<style>
</style>
