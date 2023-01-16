<script setup>
import { ScaleDataGrid } from '@telekom/scale-components/dist/components/scale-data-grid';
import { ScaleAppShell } from '@telekom/scale-components/dist/components/scale-app-shell';

if (!customElements.get('custom-scale-data-grid')) {
  customElements.define('custom-scale-data-grid', ScaleDataGrid);
}
if (!customElements.get('custom-scale-app-shell')) {
  customElements.define('custom-scale-app-shell', ScaleAppShell);
}

const fields = [
  {
    type: 'checkbox',
    label: 'Checkbox',
    style: 'checkbox',
  },
  {
    type: 'checkbox',
    label: 'Switch',
    style: 'switch',
  },
  {
    type: 'checkbox',
    label: 'Editable Checkbox',
    style: 'checkbox',
    editable: true,
    sortable: true,
  },
  {
    type: 'checkbox',
    label: 'Editable Switch',
    style: 'switch',
    editable: true,
    sortable: true,
  },
];
const rows = [
  [true, false, true, true],
  [true, true, true, false],
  [false, true, false, false],
  [false, false, false, true],
];
</script>

<template>
  <custom-scale-app-shell laim-lang="de" logo-title="App Name" logo-href="/">
    <div>
      <div>
        <custom-scale-data-grid
          :rows="rows"
          :fields="fields"
          hide-menu
          sortable
        />
        <scale-button>abc</scale-button>
      </div>
    </div>
  </custom-scale-app-shell>
</template>
