<template>
    <div>
        <div class="container">
            
            <div class="title"><h1>Informacje</h1></div>
            <p class="article">{{article}}</p>
        </div>
    </div>
</template>
<script>

export default {
    data(){
        return{
            article: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras posuere odio eu aliquam suscipit. Curabitur quis dolor aliquet, placerat augue a, venenatis tellus. Phasellus nec nulla mollis, sodales ipsum nec, venenatis tellus. Nam et finibus eros. Vestibulum tellus metus, fringilla non dapibus in, pellentesque a ante. Etiam tristique, mauris vitae tempor rutrum, mi urna pellentesque elit, in porta eros augue rutrum ex. Morbi felis elit, finibus nec augue vitae, porttitor lacinia magna. In efficitur eu arcu a tincidunt. Praesent orci est, blandit at lorem ut, viverra aliquam orci. In sed felis gravida, maximus leo quis, tincidunt dolor. Pellentesque et enim bibendum, malesuada mauris vitae, fringilla lorem. Vestibulum sit amet finibus justo. Mauris leo libero, aliquam a dapibus vel, finibus sit amet ex. Aliquam erat volutpat. Nullam tincidunt tincidunt risus vitae facilisis. Pellentesque sollicitudin pulvinar risus non condimentum. Nunc ultricies ut urna in maximus. Suspendisse ut elementum massa. Mauris mattis sapien metus, et fermentum nibh vestibulum at. Mauris finibus augue id mi vehicula, quis consectetur libero porttitor. Proin nec fermentum metus. Aliquam auctor, augue a iaculis laoreet, tellus ante aliquet sem, sit amet suscipit tortor mauris eu risus. Nulla condimentum velit non nisl accumsan congue. Interdum et malesuada fames ac ante ipsum primis in faucibus. Mauris efficitur purus et urna pulvinar, mattis vehicula tellus rutrum. Integer ex sapien, finibus vitae lobortis eu, interdum in diam. Proin dictum orci at mi hendrerit venenatis. Phasellus tincidunt, orci id elementum mollis, sem nunc porttitor lorem, et tristique neque urna ut odio. Suspendisse fermentum sapien arcu, et posuere ex mattis in. Nulla fermentum leo vel est dictum interdum. Nulla sollicitudin porta sodales. Nunc finibus auctor egestas. Sed sed mauris aliquam, condimentum felis vitae, semper felis.'
        }
    }
}
</script>
<style scoped>
 @import "~/styles/infoStyles.css" 
</style>