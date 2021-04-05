<script>
    let messages = ['M1', 'M2'];
</script>

{#each messages as msg, i }
    <p>{i}. {msg}</p>
{/each}