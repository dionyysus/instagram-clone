<template>
  <div>
    <!-- header -->

    <header class = "header section">

      <div class = "header-author">
        <Avatar size = "40"/>
        <div class="header-author-info">
          <div>
            <CustomText tag = "b">gizemcoskun</CustomText>
          </div>
          <div>
            <CustomText size ="xsmall">Istanbul, Turkey</CustomText>

          </div>

        </div>
      </div>

      <div class="header-more">
        <button type="button">
          <IconMore />
        </button>
      </div>

    </header>
    <!-- media -->

    <div class= "post-media">
      <img
          src="https://i.pinimg.com/564x/06/f4/94/06f494519ba453512de106f1f9900a89.jpg"
          alt=""
      />
    </div>
    <!-- actions -->
    <div class="action-buttons section">
      <button type="button">
        <IconLike />
      </button>
      <button type="button">
        <IconComment />
      </button>
      <button type="button">
        <IconDirect />
      </button>
      <button class = "action-save" type="button">
        <IconSave />
      </button>
    </div>
    <!-- view count -->

    <div class="view-count section">
      <custom-text tag = "b">1.345 beğenme</custom-text>
    </div>
    <!-- comment list  -->

    <!-- datetime -->

    <!-- comment form -->

  </div>
</template>

<script>
import Avatar from "./Avatar";
import CustomText from "./CustomText";
import IconMore from '@/icons/more.svg';
import IconLike from '@/icons/like.svg';
import IconComment from '@/icons/comment.svg';
import IconDirect from '@/icons/direct.svg';
import IconSave from '@/icons/save.svg';

export default {
  name: 'Post',
  components: {CustomText, Avatar,IconMore,IconLike,IconComment,IconDirect,IconSave}
}
</script>

<style scoped>
.post{
  border-radius: 3px;
  border: 1px solid rgb(var(--b6a))
}
.section {
  padding-left: 16px;
  padding-right: 16px;
}

.header{
  height: 60px;
  display: flex;
  align-items: center;
  &-author{
    display: flex;
    align-items: center;
    &-info{
      margin-left: 8px;
    }
  }
  &-more{
    margin-left: auto;
  }
}

.action-buttons {
  height: 45px;
  display: flex;
  align-items: center;

  button{
    margin-right: 16px;
  }
  .action-save{
    margin-left:auto;

  }
}

</style>