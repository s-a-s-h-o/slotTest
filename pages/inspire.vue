<template>
	<testOne>
      <div slot="head"><testTwo/></div>
      <div slot="messageBox"><testThree/></div>
	</testOne>
</template>

<script>
import testOne from "../components/testOne"
import testTwo from "../components/testTwo"
import testThree from "../components/testThree"

export default {
  components:{
    testOne,
    testTwo,
    testThree
  }
}
</script>

<style>

</style>
