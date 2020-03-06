<template>
  <div id="Footer">
      <span>{{info}}</span>
  </div>
</template>

<script>
export default {
    name: 'Footer',
    data: () => ({
      info: "� 2020 FIDE International Chess Federation. All Rights Reserved. No part of this site may be reproduced, stored in a retrieval system or transmitted in any way or by any means(including photocopying, recording or storing it in any medium by electronic means), without the written permission of FIDE International Chess Federation."
    })

}
</script>

<style lang="scss" scoped>

$color: #334166;

#Footer {
  background: $color;
  color: grey;
  text-align: center;
  padding: 20px;
}

</style>