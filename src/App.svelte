<script>
 let name = 'Max';
 let age = 30;

 $: upper = name.toUpperCase();

 function incrementAge() {
   age += 1;
 }

 function changeName() {
   name = 'filipe'
 }

</script>

<style>
 h1 {
   color: purple;
 }
</style>

<h1>Hello {upper}, my age is {age}!</h1>
<button on:click="{incrementAge}">Change Age</button>
<button on:click="{changeName}">Change name</button>
