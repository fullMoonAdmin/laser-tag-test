<script>
    let num = 0;
    let increment = ()=>{
        num++;
        console.log("number incremented");
    }
    let decrement = ()=>{
        num--;
        console.log("number decremented");
    }
</script>

<h1>Application Test</h1>

<div id="application">
<div id="number">{num}</div>

<button on:click={increment} id="increment">+</button>
<button on:click={decrement} id="decrement">-</button>
</div>
<style>
    :global(html){
        background-color: slategray;
        color: whitesmoke;
        
    }
    button{
        border-radius: 4px;
        padding: 5px;
        color: aliceblue;
        font-size: xx-large;
    }
    #application{
        text-align: center;
        border: solid 1px white;
        padding: 5px;
        font-size: 100px;
    }
    #increment{
        background-color: green;
    }
    #decrement{
        background-color: red;
    }
    
</style>
