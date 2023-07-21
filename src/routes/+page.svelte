<script lang="ts">
    import ButtonSvelte from "../components/ButtonSvelte.svelte";

    export let title: string;
    export let description: string;
  </script>
  
<div class="card">
    <img class="image" src="https://planoscelular.claro.com.br/medias/18391-0-zero-300Wx300H-productCard?context=bWFzdGVyfGltYWdlc3w2OTc0NHxpbWFnZS9wbmd8aGNkL2hmZi85MjY3OTY0MDE4NzE4LzE4MzkxXzBfemVyb18zMDBXeDMwMEhfcHJvZHVjdENhcmR8NGI3NDdjMWIyYWYwODEzZTQwYTY3YzRhOTc3NTc2NGFiZWJiYzBkOThlNWYwYTM4ODkwYzM3MTJlZjYwYmEzNA" alt="Product Image" />
    <div class="title">{title}</div>
    <div class="description">{description}</div>
    <div class="buttons">
        <a href="/product">
            <ButtonSvelte>Details</ButtonSvelte>
        </a>
      <button class="button">Add to Cart</button>
    </div>
  </div>


  <style>
    .card {
      border: 1px solid #ccc;
      border-radius: 8px;
      padding: 16px;
      margin-bottom: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      max-width: 300px;
    }
  
    .image {
      width: 200px;
      height: 200px;
      border-radius: 8px;
      object-fit: cover;
      margin-bottom: 16px;
    }
  
    .title {
      font-size: 20px;
      font-weight: bold;
      margin-bottom: 8px;
    }
  
    .description {
      text-align: center;
      margin-bottom: 16px;
    }
  
    .buttons {
      display: flex;
      justify-content: center;
    }
  
    .button {
      margin: 8px;
      padding: 10px 20px;
      background-color: #007bff;
      color: #fff;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.2s;
    }
  
    .button:hover {
      background-color: #0056b3;
    }
  </style>