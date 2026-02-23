<script>
    import { onMount } from 'svelte'

    import Reveal from 'reveal.js'
    import Markdown from 'reveal.js/plugin/markdown/markdown'
    import Highlight from 'reveal.js/plugin/highlight/highlight'
    import Notes from 'reveal.js/plugin/notes/notes'

    import 'reveal.js/dist/reveal.css'
    import './white-alt.css'
    import 'reveal.js/plugin/highlight/monokai.css'

    import Cover from './slides/Cover.svelte';
    import Intro from './slides/Intro.svelte';
    import Def from './slides/Def.svelte';
    import Code from './slides/Code.svelte';
    import Activity from './slides/Activity.svelte';
    import Credits from './slides/Credits.svelte';

    onMount(() => {
        let deck = new Reveal({
            hash: true,

			width: 1280,
			height: 720,
            maxScale: 4.0,
			margin: 0,
			center: false,
			progress: false,
			slideNumber: "c/t",

            // Learn about plugins: https://revealjs.com/plugins/
            plugins: [ Markdown, Highlight, Notes ]
        });
        deck.initialize();
    })
</script>

<div class="reveal">
    <div class="slides">
        <Cover/>
        <Intro/>
        <Def/>
        <Code/>
        <Activity/>
        <Credits/>
    </div>
</div>