<script>
    let total = 0;
    let console = "";
    let state = null;
    function resolveState(){

    }
    function setOperation(operation){

    }
    function setValue(value){

    }
    function equal(){

    }
</script>

<style>

</style>

<div class="calculator">
    <input type = "text" bind:value={console} readonly="true"/>
    <div class="buttons">
        <div class="operations">
            <button onclick={()=>{setOperation('add');}}>+</button>
            <button onclick={()=>{setOperation('substract');}}>-</button>
            <button onclick={()=>{setOperation('multiply');}}>&times</button>
            <button onclick={()=>{setOperation('divide');}}>&divide</button>
        </div>
        
        <div>
            <button on:click={()=>{setValue(7);}}>7</button>
            <button on:click={()=>{setValue(8);}}>8</button>
            <button on:click={()=>{setValue(9);}}>9</button>
        </div>
        <div>
            <button on:click={()=>{setValue(4);}}>4</button>
            <button on:click={()=>{setValue(5);}}>5</button>
            <button on:click={()=>{setValue(6);}}>6</button>
        </div>
        <div>
            <button on:click={()=>{setValue(1);}}>1</button>
            <button on:click={()=>{setValue(2);}}>2</button>
            <button on:click={()=>{setValue(3);}}>3</button>
        </div>
    </div>
</div>