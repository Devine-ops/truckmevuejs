<template>
    <div class="container">
      <h2>Entre em Contato</h2>
      <div class="formulario">
        <form @submit.prevent="handleSubmit">
          <input v-model="formData.name" type="text" class="name" placeholder="Nome completo" required>
          <input v-model="formData.email" type="email" class="email" placeholder="E-mail" required>
          <textarea v-model="formData.message" class="mensagem" placeholder="Deixa sua mensagem!" required></textarea>
          <button type="submit" class="envia">Enviar!</button>
        </form>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ContactFormComponent',
    data() {
      return {
        formData: {
          name: '',
          email: '',
          message: ''
        }
      };
    },
    methods: {
      handleSubmit() {
        if (this.formData.name && this.formData.email && this.formData.message) {
          alert('Formulário enviado com sucesso!');
          this.resetForm();
        }
      },
      resetForm() {
        // Limpar os dados do formulário após o envio
        this.formData.name = '';
        this.formData.email = '';
        this.formData.message = '';
      }
    }
  };
  </script>