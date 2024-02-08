<script>
    let username = '';
    let password = '';
    
    function handleSubmit() {
        console.log("Username:", username);
        console.log("Password:", password);
        }
</script>

<main>
    <h1>SeyfertSoft Solutions</h1>
    <form on:submit|preventDefault={handleSubmit}>
        <label for="username">Username:</label><br>
        <input type="text" id="username" bind:value={username}><br>
        
        <label for="password">Password:</label><br>
        <input type="password" id="password" bind:value={password}><br>
        
        <button type="submit">Login</button>
    </form>
</main>

<style>
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }
    
    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 2em;
        font-weight: 100;
    }
    
    form {
        margin-top: 1em;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    
    label {
        margin-bottom: 0.5em;
    }
    
    input {
        padding: 0.5em;
        margin-bottom: 1em;
        width: 100%;
    }
    
    button {
        padding: 0.5em 1em;
        background-color: #ff3e00;
        color: white;
        border: none;
        cursor: pointer;
    }
    
    button:hover {
        background-color: #ff5f33;
    }
</style>
