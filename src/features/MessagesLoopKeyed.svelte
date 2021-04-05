<script>
    let messages = [
        {id: 10, text: 'M1'},
        {id: 11, text: 'M2'},
        {id: 12, text: 'M3'},
    ];

    setTimeout(() => {
        messages = messages.slice(0,2);
    }, 2000);
</script>

{#each messages as msg (msg.id)}
    <p>{msg.text}</p>
{/each}