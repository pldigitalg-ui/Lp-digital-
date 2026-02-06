<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>PL Digital Marketing | Gestão de Páginas & Tráfego Pago</title>

  <!-- SEO / Compartilhamento -->
  <meta name="description" content="PL Digital Marketing: gestão de páginas, tráfego pago e estratégia para gerar clientes no WhatsApp.">
  <meta property="og:title" content="PL Digital Marketing">
  <meta property="og:description" content="Gestão de páginas + anúncios para gerar clientes todos os dias. Sem contrato de fidelidade.">
  <meta property="og:type" content="website">

  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

  <style>
    body{background:#f6f7fb;min-height:100vh}
    .wrap{max-width:980px;margin:28px auto;padding:0 14px}
    .card{border:0;border-radius:20px;box-shadow:0 14px 40px rgba(0,0,0,.10)}
    .left{
      background: linear-gradient(135deg, #0d6efd, #083b93);
      color:#fff;border-radius:18px;padding:26px;
      min-height:100%;
    }
    .logo{width:150px;height:auto;display:block}
    .muted{color:#6c757d}
    .pill{
      display:inline-block;padding:6px 10px;border-radius:999px;
      background:rgba(255,255,255,.12);color:#fff;font-weight:600;font-size:.9rem
    }
    .benefit{display:flex;gap:10px;align-items:flex-start}
    .dot{
      width:10px;height:10px;border-radius:999px;background:#fff;opacity:.9;margin-top:7px
    }
    .form-control{border-radius:12px;padding:12px 14px}
    .btn-primary{border-radius:12px;padding:12px 14px;font-weight:800}
    .mini{font-size:.92rem}
    .whats{
      position:fixed;right:18px;bottom:18px;z-index:9999;text-decoration:none;
    }
    .whats .btn{
      border-radius:999px;padding:12px 16px;
      box-shadow:0 10px 25px rgba(0,0,0,.18);
      font-weight:800
    }
    .trust{
      border-radius:14px;
      background:#f1f5ff;
      padding:12px 14px;
      font-size:.93rem;
      color:#1f3b7a;
    }
  </style>
</head>

<body>
  <div class="wrap">
    <div class="card p-3 p-md-4">
      <div class="row g-3 g-md-4 align-items-stretch">

        <!-- COLUNA ESQUERDA (COPY) -->
        <div class="col-12 col-lg-6">
          <div class="left h-100">
            <img class="logo mb-3" src="logo.jpeg?v=1" alt="PL Digital Marketing"
                 onerror="this.style.display='none'; document.getElementById('logoError').classList.remove('d-none');">

            <div id="logoError" class="d-none mt-2" style="color:rgba(255,255,255,.95)">
              Logo não carregou. Confirme se o arquivo <b>logo.jpeg</b> está publicado no GitHub Pages.
            </div>

            <div class="d-flex flex-wrap gap-2 mb-3">
              <span class="pill">Gestão de Páginas</span>
              <span class="pill">Tráfego Pago</span>
              <span class="pill">Instagram Profissional</span>
            </div>

            <h1 class="h3 fw-bold mb-2">
              Gestão de Instagram e anúncios para gerar clientes todos os dias.
            </h1>

            <p class="mb-4" style="opacity:.95">
              A <b>PL Digital Marketing</b> cuida da sua presença online: gestão de páginas,
              tráfego pago e estratégia focada em chamar clientes no WhatsApp.
              Sem post aleatório. Sem anúncio no escuro.
            </p>

            <div class="d-grid gap-3">
              <div class="benefit">
                <span class="dot"></span>
                <div>
                  <div class="fw-bold">Atendimento rápido no WhatsApp</div>
                  <div class="mini" style="opacity:.9">
                    Você preenche e a gente te chama com a melhor estratégia pro seu negócio.
                  </div>
                </div>
              </div>

              <div class="benefit">
                <span class="dot"></span>
                <div>
                  <div class="fw-bold">Tráfego pago que chama cliente</div>
                  <div class="mini" style="opacity:.9">
                    Anúncios no Instagram e Facebook focados em WhatsApp e conversão.
                  </div>
                </div>
              </div>

              <div class="benefit">
                <span class="dot"></span>
                <div>
                  <div class="fw-bold">Gestão profissional de páginas</div>
                  <div class="mini" style="opacity:.9">
                    Conteúdo estratégico, perfil organizado e autoridade para sua marca.
                  </div>
                </div>
              </div>
            </div>

            <hr class="my-4" style="border-color:rgba(255,255,255,.2)">

            <div class="row text-center g-2">
              <div class="col-4">
                <div class="fw-bold">+Clientes</div>
                <div class="mini" style="opacity:.9">foco em conversão</div>
              </div>
              <div class="col-4">
                <div class="fw-bold">Rápido</div>
                <div class="mini" style="opacity:.9">setup ágil</div>
              </div>
              <div class="col-4">
                <div class="fw-bold">Suporte</div>
                <div class="mini" style="opacity:.9">WhatsApp</div>
              </div>
            </div>
          </div>
        </div>

        <!-- COLUNA DIREITA (FORM) -->
        <div class="col-12 col-lg-6">
          <div class="p-3 p-md-4">
            <h2 class="h4 fw-bold mb-1">Quer clientes no Instagram e WhatsApp?</h2>
            <p class="muted mb-3">
              Preencha os dados e a PL Digital chama você com uma estratégia personalizada.
            </p>

            <div class="trust mb-4">
              ✅ Atendimento humano • ✅ Sem contrato de fidelidade • ✅ Sem spam
            </div>

            <div id="success" class="alert alert-success d-none" role="alert">
              ✅ Enviado! Já vamos te chamar no WhatsApp.
            </div>

            <form id="leadForm" novalidate>
              <div class="mb-3">
                <label class="form-label">Nome</label>
                <input name="nome" type="text" class="form-control" placeholder="Ex: Paulo Roberto" required>
                <div class="invalid-feedback">Informe seu nome.</div>
              </div>

              <div class="mb-3">
                <label class="form-label">WhatsApp (com DDD)</label>
                <input name="whatsapp" type="tel" class="form-control"
                       inputmode="numeric" autocomplete="tel"
                       placeholder="(31) 9 9806-4556" required>
                <div class="invalid-feedback">Informe seu WhatsApp.</div>
              </div>

              <div class="mb-3">
                <label class="form-label">Seu negócio</label>
                <input name="negocio" type="text" class="form-control" placeholder="Ex: Serralheria, Barbearia, Loja..." required>
                <div class="invalid-feedback">Diga qual é seu negócio.</div>
              </div>

              <div class="mb-3">
                <label class="form-label">O que você quer agora?</label>
                <select name="servico" class="form-control" required>
                  <option value="" selected disabled>Selecione</option>
                  <option>Gestão de Instagram (posts + estratégia)</option>
                  <option>Tráfego Pago (Meta/Google)</option>
                  <option>Site / Landing Page</option>
                  <option>Pacote completo (gestão + anúncios + site)</option>
                </select>
                <div class="invalid-feedback">Selecione uma opção.</div>
              </div>

              <div class="mb-3">
                <label class="form-label">Instagram (opcional)</label>
                <input name="instagram" type="text" class="form-control" placeholder="@seuinstagram">
              </div>

              <button id="btnSend" class="btn btn-primary w-100" type="submit">
                Quero gestão profissional
              </button>

              <div class="text-center mt-3">
                <a id="whatsTextLink" target="_blank" class="text-decoration-none fw-semibold"
                   href="https://wa.me/5531998064556?text=Oi%20PL%20Digital!%20Quero%20um%20or%C3%A7amento.">
                  Prefiro falar direto no WhatsApp
                </a>
              </div>

              <p class="muted text-center mt-3 mb-0 mini">
                Seus dados são usados apenas para atendimento. Sem spam.
              </p>
            </form>
          </div>
        </div>

      </div>
    </div>
  </div>

  <!-- WhatsApp flutuante (dinâmico com dados do formulário) -->
  <a class="whats" id="whatsFloat" target="_blank" href="#">
    <span class="btn btn-success">WhatsApp</span>
  </a>

  <script>
    const form = document.getElementById('leadForm');
    const btn = document.getElementById('btnSend');
    const success = document.getElementById('success');

    const whatsFloat = document.getElementById('whatsFloat');
    const whatsTextLink = document.getElementById('whatsTextLink');

    function buildWhatsLink() {
      const nome = (form.nome?.value || '').trim();
      const whatsapp = (form.whatsapp?.value || '').trim();
      const negocio = (form.negocio?.value || '').trim();
      const servico = (form.servico?.value || '').trim();
      const insta = (form.instagram?.value || '').trim();

      const msg =
        `Oi PL Digital! Quero gestão de páginas e marketing.\n\n` +
        `Nome: ${nome}\n` +
        `WhatsApp: ${whatsapp}\n` +
        `Negócio: ${negocio}\n` +
        `Interesse: ${servico}\n` +
        (insta ? `Instagram: ${insta}\n` : '');

      const url = `https://wa.me/5531998064556?text=${encodeURIComponent(msg)}`;
      whatsFloat.href = url;
      whatsTextLink.href = url;
    }

    form.addEventListener('input', buildWhatsLink);
    buildWhatsLink();

    form.addEventListener('submit', (e) => {
      e.preventDefault();

      if (!form.checkValidity()) {
        form.classList.add('was-validated');
        return;
      }

      btn.disabled = true;
      const old = btn.innerText;
      btn.innerText = 'Enviando...';

      // Aqui você pode integrar EmailJS depois.
      setTimeout(() => {
        success.classList.remove('d-none');
        btn.disabled = false;
        btn.innerText = old;
        form.reset();
        form.classList.remove('was-validated');
        buildWhatsLink();
      }, 700);
    });
  </script>
</body>
</html>
