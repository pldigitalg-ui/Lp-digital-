



<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Cadastro de Contato</title>

    <!-- Bootstrap -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

    <link rel="stylesheet" href="style.css">

    <!-- EmailJS -->
    <script src="https://cdn.jsdelivr.net/npm/emailjs-com@3/dist/email.min.js"></script>
</head>
<body>

<div class="container mt-5">
    <div class="card shadow p-4">

        <!-- Cabeçalho -->
        <div class="text-center mb-4">
            <img src="https://drive.google.com/uc?export=view&id=1EH-NNIvaef15JckxMWMt8vWBFH9y73W1" width="140" alt="PL Digital">
            <h4>Preencha seus dados para entrarmos em contato</h4>
        </div>

        <!-- Formulário -->
        <form id="formContato">
            <div class="mb-3">
                <label>Nome e Sobrenome</label>
                <input type="text" class="form-control" id="nome" required>
            </div>

            <div class="mb-3">
                <label>Email</label>
                <input type="email" class="form-control" id="email" required>
            </div>

            <div class="mb-3">
                <label>Celular (WhatsApp)</label>
                <input type="text" class="form-control" id="celular" placeholder="(99)9.9999-9999" required>
            </div>

            <div class="mb-3">
                <label>Instagram (@)</label>
                <input type="text" class="form-control" id="instagram" required>
            </div>

            <button type="submit" class="btn btn-primary w-100">
                Enviar Dados
            </button>
        </form>

    </div>
</div>

<script src="script.js"></script>
</body>
</html>
