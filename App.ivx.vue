<template>
  <ivx-stage _id="stage" width="100%" height="100%" backgroundColor="#FFFFFF" :fonts="{}" :pageCustomIdList="[]" :classStyles="{}" @load="stage_load">
    <!-- 应用系统 -->
    <ivx-system _id="system"/>
    <!-- 视频流1 -->
    <ivx-mediaStream _id="mediaStream"/>
    <!-- 按钮1 -->
    <ivx-button _id="button" bgColor="#468CF0" borderRadius="4px" :borderWidth="0" disabledBgColor="#E1E1E1" fontColor="#FFFFFF" :fontSize="14" height="34px" iconColor="#FFFFFF" :iconMargin="5" :iconSize="12" :marginBottom="12" :marginLeft="12" :marginRight="12" :marginTop="12" width="96px" @tap="button_tap"/>
    <!-- 图片1 -->
    <ivx-image _id="image" height="300px" :marginBottom="12" :marginLeft="12" :marginRight="12" :marginTop="12" :textStyle="0" width="300px"/>
  </ivx-stage>
</template>

<script>
async function stage_load() {
 let cv00shea3j50000a8rb0Rtn = $refs.cv00sgpa3j50000a8ra0.c_getUserMedia({video:"default",videoDeviceId:undefined,audio:false});
}

async function button_tap() {
 let cv25amaa3j50000rsyh0Rtn = $refs.cv00sgpa3j50000a8ra0.c_extractFrame({download:false});
 $refs.cv25b54a3j50000rsyj0.c_setSrc(cv25amaa3j50000rsyh0Rtn.result.frame);
}
</script>
