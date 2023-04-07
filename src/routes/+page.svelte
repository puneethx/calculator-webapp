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
    .calculator{
        position:absolute;
        top:50%;
        left:50%;
        transform:translate(-50%,-50%);
        width:300px;
        border:1px solid #eee;
        box-shadow:2px 2px 2px #eee;
        padding:10px;
    }
    .calculator input {
        width:100%;
        padding:20px;
        outline:none;
        text-align: right;
        font-size:20px;
    }
    .calculator .buttons{
        display:flex;
        flex-wrap: wrap;
    }
    .calculator .buttons .operations{
        display:flex;
        justify-content: space-between;
        width:100%;
    }
    .calculator .buttons .operations button{
        width:24%;
    }
    .calculator .buttons .numbers {
        width:75%;
    }
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
        
        <div class = "numbers">
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
            <div>
                <button on:click={()=>{setValue(0);}}>0</button>
                <button on:click={()=>{setValue('.');}}>2</button>
                <button on:click={()=>{setValue('C');}}>C</button>
            </div>
        </div>

        <div class = "equal">
            <button on:click={equal}>=</button>
        </div>
    </div>
</div>