<template>

  <div class="">

  </div>
</template>

<script>

const algosdk = require('algosdk');
const IPFS = require('ipfs');

async function main () {
  const node = await IPFS.create()
  const version = await node.version()

  console.log('Version:', version.version)
  // ...
}

main()

// const node = new IPFS();

//node.on('ready', () => {
  // Ready to use!
  // See https://github.com/ipfs/js-ipfs#core-api
//})

let account = algosdk.generateAccount();
console.log("Account Address: ", account.addr);

let mn = algosdk.secretKeyToMnemonic(account.sk);
console.log("Account Mnemonic: ", mn);

export default {
  name: 'SandBox',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
