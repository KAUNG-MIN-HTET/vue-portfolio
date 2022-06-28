<template>
    <div class="w-100 h-100 grid-cus">
        <ul class="animate__animated animate__rubberBand">
		<li style="--i:6;"><router-link to="/" @click="$emit('chg-title', 'home')">Home</router-link></li>
		<li style="--i:5;"><router-link to="/about" @click="$emit('chg-title', 'about')">About</router-link></li>
		<li style="--i:4;"><router-link to="/projects" @click="$emit('chg-title', 'projects')">Projects</router-link></li>
		<li style="--i:3;"><router-link to="/resume" @click="$emit('chg-title', 'resume')">Resume</router-link></li>
		<li style="--i:2;"><router-link to="/contact" @click="$emit('chg-title', 'contact')">Contact</router-link></li>
		<li style="--i:1;"><router-link to="/created" @click="$emit('chg-title', 'created')">Created</router-link></li>
	</ul>
    </div>
</template>

<script>
export default {
    name: 'LinkComponent',
    data() {
        return {
           
        }
    },
}
</script>

<style lang="scss" scoped>
    .grid-cus {
        display: grid;
        place-items: center;
    }
</style>