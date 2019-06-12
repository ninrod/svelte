<script>
 let name = 'Max';
 let age = 30;

 $: upper = name.toUpperCase();
 $: console.log(name);

 function incrementAge() {
   age += 1;
 }

 function changeName(event) {
   name = event.target.value
 }

</script>

<style>
 h1 {
   color: purple;
 }
</style>

<h1>Hello {upper}, my age is {age}!</h1>
<button on:click="{incrementAge}">Change Age</button>
<input type="text" value="{name}" on:input="{changeName}"/>
