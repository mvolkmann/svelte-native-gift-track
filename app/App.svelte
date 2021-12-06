<script lang="typescript">
  import {BottomNavigation} from '@nativescript/core';

  let message: string = 'Hello, World!';
</script>

<page>
  <actionBar title="Gift Track" />
  <gridLayout>
    <label
      class="info"
      horizontalAlignment="center"
      verticalAlignment="middle"
      textWrap="true"
    >
      <formattedString>
        <span class="fas" text="&#xf135;" />
        <span text=" {message}" />
      </formattedString>
    </label>
  </gridLayout>
</page>

<style>
  .info .fas {
    color: #3a53ff;
  }
  .info {
    font-size: 20;
  }
</style>
