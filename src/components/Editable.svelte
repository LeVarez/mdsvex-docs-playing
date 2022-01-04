<script>
    import './defineProcess.js';
    import { NodeViewWrapper, editable } from 'svelte-tiptap';
  </script>

  <NodeViewWrapper class="svelte-component">
    <span class="label">Svelte Editable Component</span>

    <p use:editable class="content editable" />
  </NodeViewWrapper>
