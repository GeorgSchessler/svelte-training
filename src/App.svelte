<script>
	import ButtonSimple from './basics/ButtonSimple.svelte';
	import ButtonJS from './basics/ButtonJS.svelte';
	import ButtonStyle from './basics/ButtonStyle.svelte';
	import Registration from './basics/Registration.svelte';

	import ButtonProps from './features/ButtonProps.svelte';
	import ButtonOpt from './features/ButtonOpt.svelte';

	import Messages from './features/Messages.svelte';
	import MessagesLoop from './features/MessagesLoop.svelte';
	import MessagesLoopIndex from './features/MessagesLoopIndex.svelte';
	import MessagesLoopKeyed from './features/MessagesLoopKeyed.svelte';
	
	import Await from './features/Await.svelte';
	import AwaitError from './features/AwaitError.svelte';

	const obj = {
		text: "Custom Button",
		title: "Custom Title"
	};
</script>

<main>
	<h1>Basics</h1>

	<h3>Simple button</h3>
	<ButtonSimple />
	<h3>Button with JavaScript</h3>
	<ButtonJS />
	<h3>Button with Styles</h3>
	<ButtonStyle />
	<h3>Registration</h3>
	<Registration />

	<h1>Features</h1>

	<h3>Properties</h3>
	<ButtonProps text="Custom Button" title="Custom Title"/>
	<h3>Spread Properties</h3>
	<ButtonProps {...obj} />
	<h3>Optimized Properties</h3>
	<ButtonProps {...obj} />
	<Messages />
	<MessagesLoop />
	<MessagesLoopIndex />
	<MessagesLoopKeyed />
	<Await />
	<AwaitError />
</main>