<template>
  <div class="main">
    <div class="left-panel">
      <img src="../assets/image-product-desktop.jpg" alt="Product Image" />
    </div>
    <div class="right-panel">
      <header>PERFUME</header>
      <h1>Gabrielle Essence Eau De Parfum</h1>
      <p>
        A floral solar and voluptuous interpretation composed by Olivier Polge,
        Perfumer-Creator for the House of CHANNEL<br />
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut similique
        facere, voluptas maxime rerum, provident exercitationem quo quas
        officia, dignissimos qui? Deserunt iusto facilis beatae. Alias eaque
        esse nam est.
      </p>
      <div class="amount">
        <span class="amt">$149.99</span>
        <span class="previousAmt">$169.99</span>
      </div>
      <button>
        <svg width="15" height="16" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M14.383 10.388a2.397 2.397 0 0 0-1.518-2.222l1.494-5.593a.8.8 0 0 0-.144-.695.8.8 0 0 0-.631-.28H2.637L2.373.591A.8.8 0 0 0 1.598 0H0v1.598h.983l1.982 7.4a.8.8 0 0 0 .799.59h8.222a.8.8 0 0 1 0 1.599H1.598a.8.8 0 1 0 0 1.598h.943a2.397 2.397 0 1 0 4.507 0h1.885a2.397 2.397 0 1 0 4.331-.376 2.397 2.397 0 0 0 1.12-2.021ZM11.26 7.99H4.395L3.068 3.196h9.477L11.26 7.991Zm-6.465 6.392a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Zm6.393 0a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Z"
            fill="#FFF"
          />
        </svg>
        <span>Add to Cart</span>
      </button>
    </div>
  </div>
</template>

<script setup></script>

<style>
.main {
  width: 80%;
  height: 80%;
  position: absolute;
  background: hsl(30, 38%, 92%);
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 20px;
}

.left-panel {
  width: 30%;
  height: 80%;
  /* background: red; */
}
.right-panel {
  background: hsl(0, 0%, 100%);
  width: 30%;
  height: 80%;
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
}

.right-panel header {
  margin: 20px 10px;
  letter-spacing: 2px;
}

.right-panel p {
  /* font-family: "Fraunces", serif; */
  font-family: "Montserrat", sans-serif;
}

.right-panel h1 {
  font-family: "Fraunces", serif;
}

.right-panel h1,
p,
.amount {
  margin: 25px 10px;
}
.right-panel p {
  font-size: 14px;
  font-family: "Montserrat", sans-serif;
}

.amount {
  margin: 0 10px 10px 20px;
  /* background-color: red; */
}

.right-panel .amt {
  font-size: xx-large;
  margin: 0 20px 0 0;
  color: hsl(158, 36%, 37%);
  font-family: "Fraunces", serif;
  font-weight: bold;
  font-size: 50px;
}

.right-panel .previousAmt {
  text-decoration: line-through;
  font-size: x-small;
}

button {
  width: 80%;
  margin: 0 20px;
  padding: 10px;
  border-radius: 6px;
  background-color: hsl(158, 36%, 37%);
  border: none;
  color: hsl(0, 0%, 100%);
}

button span {
  margin-left: 5px;
  overflow: hidden;
}

@media screen and (max-width: 375px) {
  .left-panel,
  .right-panel {
    overflow: hidden;
  }
}
</style>
