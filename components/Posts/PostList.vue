<template>
    <section class = "post-list">
      <PostPreview
        id="1"
        :is-admin="isAdmin"
        thumbnail ="https://previews.123rf.com/images/elen1/elen11711/elen1171100102/89714894-circuit-board-electronic-computer-hardware-technology-motherboard-digital-chip-tech-science-backgrou.jpg" 
        title="First Post"
        previewText="My first post"/>
      <PostPreview
        id="2"
        :is-admin="isAdmin"
        thumbnail ="https://previews.123rf.com/images/elen1/elen11711/elen1171100102/89714894-circuit-board-electronic-computer-hardware-technology-motherboard-digital-chip-tech-science-backgrou.jpg" 
        title="Second Post"
        previewText="My second post"/>
      <PostPreview
        id="3"
        :is-admin="isAdmin"
        thumbnail ="https://previews.123rf.com/images/elen1/elen11711/elen1171100102/89714894-circuit-board-electronic-computer-hardware-technology-motherboard-digital-chip-tech-science-backgrou.jpg" 
        title="Third Post"
        previewText="My third post"/>
    </section>
</template>

<script>
import PostPreview from '~/components/Posts/PostPreview'
export default {
    components:{
        PostPreview
    },
    props:{
        isAdmin: {
            type: Boolean,
            default: false
        }
    }
}
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
