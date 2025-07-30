<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README Animado - Tarciso</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Estilos personalizados e animações */
        body {
            font-family: 'Space Grotesk', sans-serif;
            background-color: #10101A;
            color: #E2E8F0;
            overflow-x: hidden;
        }

        /* Animação do gradiente de fundo */
        .animated-gradient {
            background: linear-gradient(-45deg, #10101A, #1a202c, #2d3748, #10101A);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Efeito de digitação */
        .typing-effect {
            border-right: .15em solid #6366F1; /* Cursor */
            white-space: nowrap;
            overflow: hidden;
            animation: typing 3.5s steps(40, end), blink-caret .75s step-end infinite;
        }

        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }

        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #6366F1; }
        }
        
        /* Animação de fade-in para seções */
        .fade-in-section {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeIn 0.8s ease-out forwards;
        }

        @keyframes fadeIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .section-1 { animation-delay: 0.5s; }
        .section-2 { animation-delay: 0.8s; }
        .section-3 { animation-delay: 1.1s; }
        .section-4 { animation-delay: 1.4s; }

        /* Estilo e animação para os cards de habilidades */
        .skill-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease, background-color 0.3s ease;
            border: 1px solid #334155;
        }

        .skill-card:hover {
            transform: translateY(-10px) scale(1.03);
            background-color: #1E293B;
            box-shadow: 0 20px 25px -5px rgba(99, 102, 241, 0.2), 0 10px 10px -5px rgba(99, 102, 241, 0.1);
        }
        
        .icon-glow {
            transition: filter 0.3s ease;
        }

        .skill-card:hover .icon-glow {
            filter: drop-shadow(0 0 8px rgba(165, 180, 252, 0.8));
        }

    </style>
</head>
<body class="animated-gradient">

    <div class="container mx-auto p-4 md:p-8 max-w-4xl">

        <!-- Seção Header -->
        <header class="text-center py-16 fade-in-section section-1">
            <h1 id="greeting" class="text-4xl md:text-6xl font-bold text-white mb-4"></h1>
            <p class="text-xl md:text-2xl text-indigo-300 font-light">Especialista UI/UX & Desenvolvedor Front-End</p>
        </header>

        <!-- Sobre Mim -->
        <section class="my-12 p-8 bg-slate-800/50 rounded-2xl border border-slate-700 fade-in-section section-2">
            <h2 class="text-3xl font-bold text-indigo-300 mb-4">Olá, mundo! 👋 Eu sou o Tarciso.</h2>
            <p class="text-slate-300 leading-relaxed">
                Sou um apaixonado por criar experiências digitais que não são apenas bonitas, mas também intuitivas e memoráveis. Minha jornada no mundo da tecnologia é movida pela união entre o design centrado no usuário e o desenvolvimento de interfaces fluidas e responsivas. Transformo ideias complexas em soluções elegantes e funcionais.
            </p>
        </section>

        <!-- Minhas Habilidades -->
        <section class="my-12 fade-in-section section-3">
            <h2 class="text-3xl font-bold text-center text-indigo-300 mb-10">Meu Arsenal de Habilidades</h2>
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
                <!-- UI/UX Design -->
                <div class="skill-card bg-slate-800/50 rounded-2xl p-6 text-center">
                    <img src="https://placehold.co/80x80/6366F1/FFFFFF?text=UI" alt="Ícone de UI/UX" class="mx-auto mb-4 h-20 w-20 rounded-full icon-glow">
                    <h3 class="font-bold text-lg text-white">UI/UX Design</h3>
                    <p class="text-sm text-slate-400">Prototipagem, Wireframing, User Flows</p>
                </div>
                <!-- HTML5 -->
                <div class="skill-card bg-slate-800/50 rounded-2xl p-6 text-center">
                     <img src="https://placehold.co/80x80/F16529/FFFFFF?text=HTML" alt="Ícone de HTML5" class="mx-auto mb-4 h-20 w-20 rounded-full icon-glow">
                    <h3 class="font-bold text-lg text-white">HTML5</h3>
                    <p class="text-sm text-slate-400">Estrutura semântica e acessível</p>
                </div>
                <!-- CSS3 -->
                <div class="skill-card bg-slate-800/50 rounded-2xl p-6 text-center">
                    <img src="https://placehold.co/80x80/2965F1/FFFFFF?text=CSS" alt="Ícone de CSS3" class="mx-auto mb-4 h-20 w-20 rounded-full icon-glow">
                    <h3 class="font-bold text-lg text-white">CSS3</h3>
                    <p class="text-sm text-slate-400">Flexbox, Grid, Animações</p>
                </div>
                <!-- JavaScript -->
                <div class="skill-card bg-slate-800/50 rounded-2xl p-6 text-center">
                    <img src="https://placehold.co/80x80/F7DF1E/000000?text=JS" alt="Ícone de JavaScript" class="mx-auto mb-4 h-20 w-20 rounded-full icon-glow">
                    <h3 class="font-bold text-lg text-white">JavaScript</h3>
                    <p class="text-sm text-slate-400">ES6+, DOM, Interatividade</p>
                </div>
                <!-- React.js -->
                <div class="skill-card bg-slate-800/50 rounded-2xl p-6 text-center">
                    <img src="https://placehold.co/80x80/61DAFB/000000?text=R" alt="Ícone de React.js" class="mx-auto mb-4 h-20 w-20 rounded-full icon-glow">
                    <h3 class="font-bold text-lg text-white">React.js</h3>
                    <p class="text-sm text-slate-400">Componentes e Hooks</p>
                </div>
                <!-- Git & GitHub -->
                <div class="skill-card bg-slate-800/50 rounded-2xl p-6 text-center">
                    <img src="https://placehold.co/80x80/181717/FFFFFF?text=Git" alt="Ícone de Git" class="mx-auto mb-4 h-20 w-20 rounded-full icon-glow">
                    <h3 class="font-bold text-lg text-white">Git & GitHub</h3>
                    <p class="text-sm text-slate-400">Versionamento de código</p>
                </div>
                <!-- APIs -->
                <div class="skill-card bg-slate-800/50 rounded-2xl p-6 text-center">
                    <img src="https://placehold.co/80x80/3B82F6/FFFFFF?text=API" alt="Ícone de API" class="mx-auto mb-4 h-20 w-20 rounded-full icon-glow">
                    <h3 class="font-bold text-lg text-white">APIs</h3>
                    <p class="text-sm text-slate-400">Integração RESTful</p>
                </div>
                <!-- Chatbots -->
                <div class="skill-card bg-slate-800/50 rounded-2xl p-6 text-center">
                    <img src="https://placehold.co/80x80/4ADE80/FFFFFF?text=Bot" alt="Ícone de Chatbot" class="mx-auto mb-4 h-20 w-20 rounded-full icon-glow">
                    <h3 class="font-bold text-lg text-white">Chatbots</h3>
                    <p class="text-sm text-slate-400">Automação de conversas</p>
                </div>
            </div>
        </section>

        <!-- Contato -->
        <section class="text-center my-16 fade-in-section section-4">
            <h2 class="text-3xl font-bold text-indigo-300 mb-4">Vamos nos Conectar?</h2>
            <p class="text-slate-300 mb-8 max-w-2xl mx-auto">Estou sempre aberto a novas oportunidades, colaborações e um bom bate-papo sobre tecnologia e design. Me encontre nas redes abaixo!</p>
            <div class="flex justify-center space-x-6">
                <a href="#" class="text-slate-400 hover:text-indigo-300 transition-colors duration-300">
                    <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path fill-rule="evenodd" d="M12 2C6.477 2 2 6.477 2 12.013c0 4.418 2.865 8.169 6.839 9.492.5.092.682-.217.682-.482 0-.237-.009-.868-.014-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.031-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.338 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.001 10.001 0 0022 12.013C22 6.477 17.523 2 12 2z" clip-rule="evenodd" /></svg>
                </a>
                <a href="#" class="text-slate-400 hover:text-indigo-300 transition-colors duration-300">
                    <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
                </a>
            </div>
        </section>
    </div>

    <script>
        // Script para o efeito de digitação
        const greetingText = "Oi, eu sou o Tarciso";
        const greetingElement = document.getElementById('greeting');
        let i = 0;

        function typeWriter() {
            if (i < greetingText.length) {
                greetingElement.innerHTML += greetingText.charAt(i);
                i++;
                setTimeout(typeWriter, 100);
            } else {
                // Remove o cursor piscando após a digitação
                greetingElement.style.borderRight = 'none';
            }
        }

        // Inicia a animação quando a página carrega
        window.onload = function() {
            // Limpa o texto inicial para o efeito de digitação
            greetingElement.innerHTML = '';
            // Adiciona a classe para o cursor
            greetingElement.classList.add('typing-effect');
            // Remove a classe após a animação para não re-digitar
            setTimeout(() => {
                 greetingElement.classList.remove('typing-effect');
                 greetingElement.style.borderRight = 'none';
            }, 3500); // Duração da animação de digitação
            
            // Substitui o texto pelo texto completo para evitar problemas de layout
            // e inicia o efeito de digitação visual
            const fullText = "Oi, eu sou o Tarciso";
            greetingElement.textContent = fullText;
        };
    </script>
</body>
</html>
