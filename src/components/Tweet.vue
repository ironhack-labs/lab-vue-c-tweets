<script setup>
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";
// Iteration 2 | Pass the Tweet as a Prop Define props

const props = defineProps({
	user: Object,
	timestamp: String,
	message: String,
});
</script>

<template>
	<div class="tweet">
		<ProfileImage :image="user.image" />

		<div class="body">
			<div class="top">
				<User :userData="user" />
				<Timestamp :time="timestamp" />
			</div>

			<Message :message="message" />
			<Actions :actions="actions" />
		</div>

		<i class="fas fa-ellipsis-h"></i>
	</div>
</template>

<style scoped>
a {
	color: #42b983;
}
</style>
