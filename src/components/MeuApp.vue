<template>
  <div class="container">
    <div class="header">
      <div class="menu">
        <router-link to="/" class="text-bold white-text">Blog</router-link>
        <router-link to="/sobre" class="text-bold white-text">Sobre</router-link>
        <router-link to="/descricao" class="text-bold white-text">Descrição</router-link>
      </div>
    </div>

    <div class="conteudo">
      <div class="perfil">
        <img src="@/assets/logo.png" alt="Perfil" class="perfil-img" />
        <div class="perfil-info">
          <h1>Meu Blog</h1>
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. 
            Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, 
            when an unknown printer took a galley of type and scrambled it to make a type 
            specimen book. It has survived not only five centuries, but also the leap into 
            electronic typesetting, remaining essentially unchanged. It was popularised in 
            the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, 
            and more recently with desktop publishing software like Aldus PageMaker including 
            versions of Lorem Ipsum.
          </p>
        </div>
      </div>

      <div class="links-container">
        <div class="links">
          <h1>Últimas do Blog</h1>
          <div class="link-item">
            <h2>Link 1</h2>
            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. 
              Lorem Ipsum has.</p>
          </div>
          <div class="link-item">
            <h2>Link 2</h2>
            <p>The industry's standard dummy text ever since the 1500s, 
              when an unknown printer took a galley of type and scrambled it to make a type 
              specimen book. It has survived not only five centuries, but also the leap into 
              electronic typesetting, remaining .</p>
          </div>
          <div class="link-item">
            <h2>Link 3</h2>
            <p>The 1960s with the release of Letraset sheets containing Lorem Ipsum passages, 
              and more recently with desktop publishing software like Aldus PageMaker including 
              versions of Lorem Ipsum..</p>
          </div>
          <div class="link-item">
            <h2>Link 4</h2>
            <p>It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, 
              and more recently with desktop publishing software.</p>
          </div>
          <div class="link-item">
            <h2>Link 5</h2>
            <p>When an unknown printer took a galley of type and scrambled it to make a type 
              specimen book. It has survived.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  background: linear-gradient(to bottom, #0D1B2A 50%, white 50%);
  padding: 20px;
  border-radius: 10px;
}

.header {
  display: flex;
  justify-content: center;
  align-items: center;
}

.menu {
  display: flex;
  gap: 20px;
}

.text-bold {
  font-weight: bold;
  color: white;
}

.white-text {
  color: white;
}

.conteudo {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 20px;

}

.perfil {
  display: flex;
  align-items: center;
  margin-top: 20px;
  margin-bottom: 250px;
}

.perfil-img {
  border-radius: 50%;
  margin-right: 20px;
}

.perfil-info {
  max-width: 500px;
  color: white;
  text-align: justify;
}

.links-container {
  flex: 1;
  background-color: white;
  padding: 20px;
  border-radius: 10px;

}

.links {

  align-items: flex-end;
  color: black;
}

.link-item {
  text-align: center;
  margin-top: 10px;
  background-color: white;
  padding: 3px;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}

.link-item:hover {
  background-color: #FFE600;
}

.link-item h2 {
  margin-bottom: 5px;
}

.link-item p {
  margin: 0;
}
</style>
