<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost"/>
        </section>
    </div>
</template>

<script>
import AdminPostForm from '~/components/Admin/AdminPostForm'

export default {
    layout: 'admin',
    components:{
        AdminPostForm
    },
    data(){
        return {
            loadedPost:{
                author: 'Zach Wright',
                title: 'My Post',
                content: 'This is the content of the post',
                thumbnailLink: 'https://previews.123rf.com/images/elen1/elen11711/elen1171100102/89714894-circuit-board-electronic-computer-hardware-technology-motherboard-digital-chip-tech-science-backgrou.jpg'
            }
        }
    }
}
</script>

<style>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>
