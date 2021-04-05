<script>
  const messagesPromise = async () => {
    const messagesList = new Array(10);
    return await new Promise(resolve => setTimeout(() => resolve(messagesList), 1000));
  };
</script>

{#await messagesPromise()}
  <p>Loading</p>
{:then messages}
  <p>{messages.length} messages</p>
{:catch error}
	<p>{error.message}</p>
{/await}