<script>
  const messagesPromise = async () => {
    return await new Promise((resolve, reject) => reject('Error'));
  };
</script>

{#await messagesPromise()}
  <p>Loading</p>
{:then messages}
  <p>{messages.length} messages</p>
{:catch error}
	<p>{error}</p>
{/await}