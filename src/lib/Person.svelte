<script>
    export let person = "john";

    // Updated automatically every time when variable person is changed
    //
    $: upperCaseName = person.toUpperCase(); // Reactive code

    function changePerson() {
        person = "michaela";
    }
</script>

<h2>Welcome to our app, {person}!</h2>
<h2>Welcome to our app, {upperCaseName}!</h2>

<button on:click={changePerson}>Change Person's Name</button>
