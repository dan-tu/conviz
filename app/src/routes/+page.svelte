<script>
    let file, canvas, viz;

    // File -> DataURL -> Image -> Canvas
    function onSelectImage(e) {
        if (e.target.files.length) {
            file = e.target.files[0];
        }
    }
</script>

<div>
    <h1>2D Convolution Visualizer</h1>
    <h2>Step 1: Upload an Image</h2>
    <form>
        <label for="sourceImg">Choose an image:</label>
        <input type="file" id="sourceImg" accept=".png, .jpeg, .jpg" required on:change={onSelectImage} />
    </form>

    {#if file}
        <h2>Step 2: Define a Filter</h2>

    {/if}
</div>

<style>


</style>
