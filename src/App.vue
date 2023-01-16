<script setup>
import { ScaleAppShell } from '@telekom/scale-components/dist/components/scale-app-shell';
if (!customElements.get('custom-scale-app-shell')) {
  customElements.define('custom-scale-app-shell', ScaleAppShell);
}
</script>

<template>
  <custom-scale-app-shell claim-lang="de" logo-title="App Name" logo-href="/">
    <div>
      Scroll to test header behavior
      <p />
      <br />
    </div>
    <div>
      Scroll more to test header behavior
      <p />
      <br />
    </div>
    <div>
      Scroll to test header behavior
      <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
    </div>
    <div>
      Scroll more to test header behavior
      <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
    </div>

    <div>
      Scroll to test header behavior
      <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
    </div>
    <br />
    <div>
      Scroll more to test header behavior
      <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
    </div>
  </custom-scale-app-shell>
</template>
