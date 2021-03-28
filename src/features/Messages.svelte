<script>
    let messages = new Array(1);
</script>

{#if messages.length > 100}
    <p>Too many messages</p>
{:else if messages.length > 0}
    <p>{messages.length} messages</p>
{:else}
    <p>No messages</p>
{/if}