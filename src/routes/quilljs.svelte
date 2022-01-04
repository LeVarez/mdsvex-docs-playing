<script>
    import { quill } from 'svelte-quill';

    let editor;

    let toolbarOptions = [
      [{ header: 1 }, { header: 2 }, "blockquote", "link", "image"],
      ["bold", "italic", "underline", "strike"],
      [{ list: "ordered" }, { align: [] }],
      ["clean"]
    ];

    let options =  {
      modules: {
        toolbar: toolbarOptions
      },
      theme: "snow",
      placeholder: "This is a Quill Example"
    }
    let content =  {html: ""};

  </script>

<svelte:head>
	<link href="//cdn.quilljs.com/1.3.6/quill.snow.css" rel="stylesheet">
</svelte:head>

<main>
  <h1>SVELTE-QUILL</h1>
  <div class="editor" use:quill={options} on:text-change={e => content = e.detail}/>

	<br />
	Resulting HTML:

	{content.html}
</main>