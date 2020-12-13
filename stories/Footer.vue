<template>
  <footer>
    <p>test</p>
    <div>
      <my-button size="small" @onClick="onLogout" label="Log out" v-if="user" />
      <my-button size="small" @onClick="onLogin" label="Log in" v-if="!user" />
      <my-button
        primary
        size="small"
        @onClick="onCreateAccount"
        label="Sign up"
        v-if="!user"
      />
    </div>
  </footer>
</template>
