<script>
	export let variant = null;
	export let size = null;
</script>

<style>
    .button {
        font-size: 1em;
        letter-spacing: .2px;
        font-family: inherit;
        display: inline-block;
        flex: 0 0 auto;
        font-weight: 600;
        position: relative;
        margin: 0 0 ;
        padding: 1em 2em;
        border: none;
        border-radius: 2em;
        outline: none;
        width: auto;
        min-height: 2em;
        min-width: 4em;
        max-width: 100%;
        background: var(--proposales-primary);
        text-align: center;
        text-decoration: none;
        color: white;
        line-height: 1.1;
        will-change: transform, background, background-position, background-size, box-shadow, color, opacity;
    }

    .button--hollow {
        color: var(--proposales-primary);
        box-shadow: 0px 0px 0px 2px var(--proposales-primary);
        background: none;
    }
    
    .button--small {
        min-height: 1.5em;
        padding: .5em 1em;
        font-size: .9em;
    }
</style>

<button
    class="button"
    class:button--hollow={variant==='hollow'}
    class:button--small={size==='small'}
>
	<slot></slot>
</button>

