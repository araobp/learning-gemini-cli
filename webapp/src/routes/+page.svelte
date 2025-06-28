<svelte:head>
  <title>Testing Gemini CLI</title>
</svelte:head>

<script>
  import "bootstrap/dist/css/bootstrap.min.css";
  import { onMount } from 'svelte';

  onMount(async () => {
    await import('bootstrap/dist/js/bootstrap.bundle.min.js');
  });
</script>

<div class="content">
  <h1>Testing Gemini CLI</h1>
  

  

  <div class="dropdown mt-3">
    <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-expanded="false">
      Select Language
    </button>
    <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton">
      <li><a class="dropdown-item" href="#">English</a></li>
      <li><a class="dropdown-item" href="#">German</a></li>
      <li><a class="dropdown-item" href="#">Japanese</a></li>
    </ul>
  </div>

  <div class="mt-3">
    <textarea class="form-control" rows="5"></textarea>
  </div>

  <div class="mt-3">
    <input type="text" class="form-control" placeholder="Enter something...">
  </div>
</div>

<style>
  .content {
    margin: 30px;
    background-color: rgba(255, 255, 255, 0.8);
    padding: 20px;
    border-radius: 10px;
  }
  :global(body) {
    background-image: url('/brick-wall.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
  }
</style>
