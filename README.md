<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Cadastro de Contato | PL Digital</title>

  <!-- Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

  <style>
    body{
      background: #f6f7fb;
      min-height: 100vh;
    }
    .wrap{
      max-width: 520px;
      margin: 40px auto;
      padding: 0 14px;
    }
    .card{
      border: 0;
      border-radius: 18px;
      box-shadow: 0 12px 30px rgba(0,0,0,.08);
    }
    .logo{
      width: 140px;
      height: auto;
      display: block;
      margin: 0 auto;
    }
    .muted{
      color: #6c757d;
      font-size: .95rem;
    }
    .btn-primary{
      border-radius: 12px;
      padding: 12px 14px;
      font-weight: 600;
    }
    .form-control{
      border-radius: 12px;
      padding: 12px 14px;
    }
    .whats{
      position: fixed;
      right: 18px;
      bottom: 18px;
      z-index: 9999;
      text-decoration: none;
    }
    .whats .btn{
      border-radius: 999px;
      padding: 12px 16px;
      box-shadow: 0 10px 25px rgba(0,0,0,.18);
      font-weight: 700;
    }
  </style>
</head>

<body>
  <div class="wrap">
    <div class="card p-4 p-md-5">
      <!-- Logo -->
      <div class="text-center mb-3">
        <!-- IMPORTANTE: o arquivo precisa existir como "logo.jpeg" na raiz do repo -->
        <img class="logo" src="logo.jpeg" alt="PL Digital"
             onerror="this.style.display='none'; document.getElementById('logoError').classList.remove('d-none');">
        <div id="logoError" class="d-none mt-2 text-danger small">
          Logo não carregou. Verifique se o arquivo <b>logo.jpeg</b> está publicado no GitHub Pages.
        </div>
      </div>

      <h1 class="h4 text-center mb-2">Preencha seus dados</h1>
      <p class="text-center muted mb-4">
        Assim que você enviar, nossa equipe entra em contato pelo WhatsApp com a melhor solução pra você.
      </p>

      <div id="success" class="alert alert-success d-none" role="alert">
        ✅ Enviado com sucesso! Já vamos te chamar no WhatsApp.
      </div>

      <form id="leadForm" novalidate>
        <div class="mb-3">
          <label class="form-label">Nome e Sobrenome</label>
          <input name="nome" type="text" class="form-control" placeholder="Ex: Paulo Roberto" required>
          <div class="invalid-feedback">Informe seu nome completo.</div>
        </div>

        <div class="mb-3">
          <label class="form-label">Email</label>
          <input name="email" type="email" class="form-control" placeholder="ex: seuemail@gmail.com" required>
          <div class="invalid-feedback">Informe um email válido.</div>
        </div>

        <div class="mb-3">
          <label class="form-label">Celular (WhatsApp)</label>
          <input name="whatsapp" type="tel" class="form-control" placeholder="(31) 9 9999-9999" required>
          <div class="invalid-feedback">Informe seu WhatsApp com DDD.</div>
        </div>

        <div class="mb-3">
          <label class="form-label">Instagram (@) (opcional)</label>
          <input name="instagram" type="text" class="form-control" placeholder="@seuinstagram">
        </div>

        <button id="btnSend" class="btn btn-primary w-100" type="submit">
          Enviar dados
        </button>

        <p class="text-center muted mt-3 mb-0">
          Ao enviar, você concorda em receber contato da PL Digital. Seus dados são usados apenas para atendimento.
        </p>
      </form>
    </div>
  </div>

  <!-- WhatsApp Flutuante -->
  <a class="whats" target="_blank"
     href="https://wa.me/553183913499?text=Oi%20PL%20Digital!%20Acabei%20de%20enviar%20meus%20dados%20no%20formul%C3%A1rio.">
    <span class="btn btn-success">WhatsApp</span>
  </a>

  <script>
    const form = document.getElementById('leadForm');
    const btn = document.getElementById('btnSend');
    const success = document.getElementById('success');

    form.addEventListener('submit', (e) => {
      e.preventDefault();

      // validação bootstrap-like
      if (!form.checkValidity()) {
        form.classList.add('was-validated');
        return;
      }

      // Aqui você pode integrar EmailJS depois.
      btn.disabled = true;
      const old = btn.innerText;
      btn.innerText = 'Enviando...';

      // Simula envio (trocaremos pelo EmailJS quando você quiser)
      setTimeout(() => {
        success.classList.remove('d-none');
        btn.disabled = false;
        btn.innerText = old;
        form.reset();
        form.classList.remove('was-validated');
      }, 700);
    });
  </script>
</body>
</html>
