<template>
  <div class="Container">
    <div class="addUserSection">
      <h1>Kullanıcı Ekle</h1>
      <form>
        <div class="labelsAndInputs">
          <div class="labels">
            <label for="name">Ad</label>
            <label for="surname">Soyad</label>
            <label for="email">E-mail</label>
          </div>
          <div class="inputs">
            <input required type="text" name="name" id="name" />
            <input required type="text" name="surname" id="surname" />
            <input required type="email" name="email" id="email" />
          </div>
        </div>
        <div>
          <button v-on:click="addUser">Kullanıcı Ekle</button>
        </div>
      </form>
    </div>
    <div id="usersSection">
      <h1>Kullanıcılar</h1>
      <div class="user">
        <img src="/img/img_avatar.png" />
        <p class="first_name">john</p>
        <p class="last_name">Doe</p>
        <p class="email">example@gmail.com</p>
      </div>
      <div class="user">
        <img src="/img/img_avatar.png" />
        <p class="first_name">john</p>
        <p class="last_name">Doe</p>
        <p class="email">example@gmail.com</p>
      </div>
      <div class="user">
        <img src="/img/img_avatar.png" />
        <p class="first_name">john</p>
        <p class="last_name">Doe</p>
        <p class="email">example@gmail.com</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    addUser: function() {
      const usersSection = document.getElementById("usersSection");
      const img = document.createElement("img");
      img.src = "/img/img_avatar.png";
      img.style.width = "100px";
      img.style.height = "100px";
      img.style.borderRadius = "50%";
      const div = document.createElement("div");
      div.setAttribute("class", "user");
      const name = document.createElement("p");
      const surname = document.createElement("p");
      const email = document.createElement("p");
      const nametext = document.createTextNode(
        document.getElementById("name").value
      );
      const surnametext = document.createTextNode(
        document.getElementById("surname").value
      );
      const emailtext = document.createTextNode(
        document.getElementById("email").value
      );
      name.appendChild(nametext);
      surname.appendChild(surnametext);
      email.appendChild(emailtext);
      name.style.marginLeft = "15px";
      surname.style.marginLeft = "15px";
      email.style.marginLeft = "15px";
      div.appendChild(img);
      div.appendChild(name);
      div.appendChild(surname);
      div.appendChild(email);

      usersSection.appendChild(div);
      div.style.display = "flex";
      div.style.webkitFlexDirection = "row";
      div.style.alignItems = "center";
      div.style.marginLeft = "200px";
      div.style.marginTop = "25px";
    }
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap");

* {
  margin: 0;
  padding: 0;
  font-family: "Roboto Mono", monospace;
}
.Container h1 {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 220px;
}
.user img {
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
.user p {
  margin-left: 15px;
}
.user {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-left: 200px;
  margin-top: 25px;
}
.Container {
  display: flex;
  flex-direction: row;
}
.usersSection {
  display: flex;
  flex-direction: column;
}
form {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  margin-top: 40px;
}
.labels {
  display: flex;
  flex-direction: column;
}
.inputs {
  display: flex;
  flex-direction: column;
  margin-left: 25px;
}
.inputs input {
  margin-top: 10px;
  border-radius: 5px;
  border: 1px solid black;
}
.labelsAndInputs {
  display: flex;
  flex-direction: row;
}
.labels label {
  margin-top: 10px;
}
form button {
  cursor: pointer;
  margin-top: 10px;
  border-radius: 30px;
  width: 150px;
  height: 35px;
  border: solid transparent;
  background-color: #50a2a7;
  color: white;
  transition: 400ms all;
}
form button:hover {
  background-color: #e9b44c;
}
</style>