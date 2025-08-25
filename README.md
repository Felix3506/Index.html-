# Index.html-
Página de vendas <!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emagrecedor - Emagreça de Forma Natural | E-book</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #27ae60;
            --primary-dark: #219653;
            --secondary: #e74c3c;
            --accent: #f39c12;
            --light: #f8f9fa;
            --dark: #2c3e50;
            --gray: #6c757d;
            --light-green: #e8f5e9;
            --light-blue: #e3f2fd;
            --light-orange: #fff3e0;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f5fbf8;
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            color: white;
            padding: 30px 15px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="" viewBox="0 0 100 100" width="100" height="100" opacity="0.05"><circle cx="50" cy="50" r="40" fill="white"/></svg>');
            background-size: 200px;
            background-repeat: repeat;
        }

        .logo {
            font-size: 2.5rem;
            margin-bottom: 10px;
            position: relative;
        }

        h1 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            position: relative;
            line-height: 1.3;
        }

        h2 {
            font-size: 1.6rem;
            margin: 20px 0 15px;
            color: var(--dark);
            position: relative;
            line-height: 1.3;
        }

        h3 {
            font-size: 1.3rem;
            margin: 15px 0 10px;
            color: var(--dark);
            line-height: 1.3;
        }

        p {
            margin-bottom: 15px;
            font-size: 1rem;
            line-height: 1.5;
        }

        /* Buttons */
        .cta-button {
            display: inline-block;
            background-color: var(--secondary);
            color: white;
            padding: 16px 30px;
            font-size: 1.1rem;
            font-weight: bold;
            text-decoration: none;
            border-radius: 50px;
            margin: 20px 0;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
            border: none;
            cursor: pointer;
            position: relative;
            z-index: 2;
            width: 100%;
            max-width: 320px;
        }

        .cta-button:hover {
            background-color: #c0392b;
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.25);
        }

        .cta-button:active {
            transform: translateY(1px);
        }

        /* Sections */
        .section {
            padding: 40px 0;
            background-color: white;
            margin: 20px 0;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            position: relative;
        }

        .section-alt {
            background-color: var(--light-green);
        }

        .center {
            text-align: center;
        }

        /* Benefits */
        .benefits {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            margin: 25px 0;
        }

        .benefit-item {
            background-color: var(--light);
            padding: 20px;
            border-radius: 10px;
            border-left: 5px solid var(--primary);
            transition: transform 0.3s;
            text-align: center;
        }

        .benefit-item:hover {
            transform: translateY(-5px);
        }

        /* Results */
        .results {
            display: grid;
            grid-template-columns: 1fr;
            gap: 15px;
            text-align: center;
            margin: 25px 0;
        }

        .result-item {
            padding: 20px 15px;
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            border-radius: 10px;
            color: white;
        }

        .result-number {
            font-size: 2rem;
            font-weight: bold;
            margin-bottom: 8px;
        }

        /* Testimonials */
        .testimonials {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            margin: 25px 0;
        }

        .testimonial {
            background-color: var(--light);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
        }

        .testimonial-header {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }

        .testimonial-avatar {
            width: 45px;
            height: 45px;
            background-color: #ddd;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 1.3rem;
            margin-right: 12px;
            color: var(--dark);
        }

        .stars {
            color: #f1c40f;
            font-size: 1.1rem;
            margin: 8px 0;
        }

        /* Bonuses */
        .bonuses {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            margin: 25px 0;
        }

        .bonus-item {
            background: linear-gradient(135deg, var(--light-blue), #bbdefb);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s;
        }

        .bonus-item:hover {
            transform: translateY(-5px);
        }

        .bonus-icon {
            font-size: 2.5rem;
            margin-bottom: 12px;
            color: var(--primary);
        }

        /* Guarantee */
        .guarantee {
            text-align: center;
            background: linear-gradient(135deg, var(--light-orange), #ffe0b2);
            padding: 30px 20px;
            border-radius: 10px;
            margin: 25px 0;
            position: relative;
            overflow: hidden;
        }

        .guarantee-number {
            font-size: 3rem;
            font-weight: bold;
            color: var(--secondary);
            line-height: 1;
            margin-bottom: 15px;
        }

        /* FAQ */
        .faq-item {
            margin-bottom: 20px;
            border-bottom: 1px solid #eee;
            padding-bottom: 20px;
        }

        /* Offer */
        .offer {
            text-align: center;
            background: linear-gradient(135deg, #ffebee, #ffcdd2);
            padding: 30px 20px;
            border-radius: 10px;
            margin: 25px 0;
            position: relative;
            overflow: hidden;
        }

        .price {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            gap: 10px;
            margin: 20px 0;
        }

        .old-price {
            font-size: 1.5rem;
            text-decoration: line-through;
            color: var(--gray);
        }

        .new-price {
            font-size: 2.2rem;
            font-weight: bold;
            color: var(--secondary);
        }

        .features {
            text-align: left;
            max-width: 100%;
            margin: 0 auto;
        }

        .feature-item {
            display: flex;
            align-items: center;
            margin-bottom: 12px;
            font-size: 0.95rem;
        }

        .checkmark {
            color: var(--primary);
            font-weight: bold;
            margin-right: 10px;
            font-size: 1.3rem;
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 25px 0;
            text-align: center;
            margin-top: 40px;
        }

        .footer-links {
            margin-top: 15px;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }

        .footer-links a {
            color: white;
            margin: 0 8px;
            text-decoration: none;
            font-size: 0.9rem;
        }

        .footer-links a:hover {
            text-decoration: underline;
        }

        .highlight {
            color: var(--primary);
            font-weight: bold;
        }

        /* Countdown Timer */
        .countdown {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
        }

        .countdown-item {
            background: var(--dark);
            color: white;
            padding: 8px;
            border-radius: 5px;
            min-width: 60px;
        }

        .countdown-number {
            font-size: 1.5rem;
            font-weight: bold;
        }

        /* Payment Badges */
        .payment-badges {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            gap: 8px;
            margin: 15px 0;
        }

        .payment-badge {
            background: white;
            padding: 8px 15px;
            border-radius: 5px;
            font-size: 0.85rem;
            display: flex;
            align-items: center;
            gap: 5px;
            width: fit-content;
        }

        /* Checklist items */
        .checklist {
            list-style-type: none;
            padding-left: 0;
        }

        .checklist li {
            margin-bottom: 15px;
            padding-left: 35px;
            position: relative;
        }

        .checklist li:before {
            content: "☑️";
            position: absolute;
            left: 0;
            top: 0;
            font-size: 1.5rem;
        }

        /* Animation */
        @keyframes pulse {
            0% {
                transform: scale(1);
            }

            50% {
                transform: scale(1.05);
            }

            100% {
                transform: scale(1);
            }
        }

        .pulse {
            animation: pulse 2s infinite;
        }

        /* Mobile Navigation (if needed in future) */
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: white;
            cursor: pointer;
            position: absolute;
            top: 20px;
            right: 20px;
            z-index: 1000;
        }

        /* Media Queries for Larger Screens */
        @media (min-width: 768px) {
            .container {
                padding: 0 20px;
            }

            header {
                padding: 60px 20px;
            }

            h1 {
                font-size: 2.5rem;
            }

            h2 {
                font-size: 2rem;
            }

            h3 {
                font-size: 1.5rem;
            }

            .cta-button {
                font-size: 1.2rem;
                padding: 18px 35px;
                max-width: none;
                width: auto;
            }

            .section {
                padding: 60px 0;
                margin: 30px 0;
            }

            .benefits {
                grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
                gap: 25px;
            }

            .results {
                grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
                gap: 20px;
            }

            .testimonials {
                grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
                gap: 25px;
            }

            .bonuses {
                grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
                gap: 25px;
            }

            .price {
                flex-direction: row;
                gap: 20px;
            }

            .payment-badges {
                flex-direction: row;
                gap: 10px;
            }

            .guarantee {
                padding: 40px;
            }

            .offer {
                padding: 40px;
            }
        }

        /* Media Queries for Even Larger Screens */
        @media (min-width: 992px) {
            .container {
                padding: 0 30px;
            }

            .testimonials {
                grid-template-columns: repeat(3, 1fr);
            }

            .benefits {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        /* Mobile-specific adjustments */
        @media (max-width: 600px) {
            header {
                padding: 20px 10px;
            }

            .logo {
                font-size: 2rem;
            }

            h1 {
                font-size: 1.6rem;
            }

            .cta-button {
                font-size: 1rem;
                padding: 14px 25px;
            }

            .payment-badges {
                flex-direction: column;
            }
        }
    </style>
</head>

<body>
    <header>
        <div class="container">
            <div class="logo">🌱</div>
            <h1>Emagreça de Forma 100% Natural e Saudável!</h1>
            <p>Descubra o método simples, prático e eficaz para perder peso sem dietas malucas nem remédios prejudiciais.</p>
            <a href="" class="cta-button pulse">QUERO EMAGRECER AGORA!</a>
            <div class="payment-badges">
                <div class="payment-badge"><i class="fas fa-lock"></i> Pagamento Seguro</div>
                <div class="payment-badge"><i class="fas fa-shield-alt"></i> Site Protegido</div>
            </div>
        </div>
    </header>

    <div class="container">
        <section class="section">
            <h2 class="center">✅ O Que Você Vai Aprender:</h2>
            <ul class="checklist">
                <li>
                    <h3>Receitas naturais</h3>
                    <p>Que aceleram o metabolismo em até 40%</p>
                </li>
                <li>
                    <h3>Controle da fome emocional</h3>
                    <p>Sem sofrimento</p>
                </li>
                <li>
                    <h3>Hidratação correta</h3>
                    <p>O segredo para eliminar toxinas</p>
                </li>
                <li>
                    <h3>Hábitos matinais</h3>
                    <p>Para ter mais energia o dia todo</p>
                </li>
                <li>
                    <h3>Técnicas de relaxamento</h3>
                    <p>Para reduzir o cortisol (hormônio do estresse)</p>
                </li>
            </ul>

            <div class="center">
                <a href="" class="cta-button">QUERO RECEBER ESTES BENEFÍCIOS!</a>
            </div>
        </section>

        <section class="section section-alt">
            <h2 class="center">🔥 Por Que Este Método Funciona?</h2>
            <ul class="features">
                <li class="feature-item"><span class="checkmark">✔</span> Técnicas baseadas em estudos científicos da nutrição funcional</li>
                <li class="feature-item"><span class="checkmark">✔</span> Resultados sustentáveis, sem efeito sanfona</li>
                <li class="feature-item"><span class="checkmark">✔</span> Adaptável a qualquer rotina, mesmo para quem tem pouco tempo</li>
                <li class="feature-item"><span class="checkmark">✔</span> Não precisa cortar completamente seus alimentos favoritos</li>
                <li class="feature-item"><span class="checkmark">✔</span> Foco na saúde integral, não apenas no peso</li>
            </ul>
        </section>

        <section class="section">
            <h2 class="center">📈 Resultados Reais em Apenas 30 Dias</h2>
            <div class="results">
                <div class="result-item">
                    <div class="result-number">5-7kg</div>
                    <p>Perda de peso média</p>
                </div>
                <div class="result-item">
                    <div class="result-number">83%</div>
                    <p>Redução no desejo por doces</p>
                </div>
                <div class="result-item">
                    <div class="result-number">2x</div>
                    <p>Mais energia no dia a dia</p>
                </div>
            </div>

            <p class="center">✨ Mais de <span class="highlight">3.200 pessoas</span> já transformaram seus corpos e saúde com este método. Você pode ser o próximo caso de sucesso!</p>

            <div class="center">
                <a href="" class="cta-button">QUERO MEU E-BOOK AGORA!</a>
            </div>
        </section>

        <section class="section section-alt">
            <h2 class="center">💬 O Que Nossos Leitores Dizem</h2>
            <div class="testimonials">
                <div class="testimonial">
                    <div class="testimonial-header">
                        <div class="testimonial-avatar">A</div>
                        <div>
                            <h3>Ana Clara, 32 anos</h3>
                            <div class="stars">★ ★ ★ ★ ★</div>
                        </div>
                    </div>
                    <p>"Perdi 7kg em apenas 5 semanas seguindo o método! O melhor é que não senti fome e nem precisei cortar completamente o que gosto. Aprendi a ter equilíbrio e hoje me sinto muito mais
                        disposta!"</p>
                    <p><strong>Antes: 78kg | Depois: 71kg</strong></p>
                </div>

                <div class="testimonial">
                    <div class="testimonial-header">
                        <div class="testimonial-avatar">C</div>
                        <div>
                            <h3>Carlos, 41 anos</h3>
                            <div class="stars">★ ★ ★ ★ ★</div>
                        </div>
                    </div>
                    <p>"Sempre tentei dietas radicais e falhava. Com esse e-book aprendi a mudar meus hábitos de forma gradual. Em 2 meses perdi 9kg e o mais importante: mantive o peso por mais de 1 ano!"
                    </p>
                    <p><strong>Antes: 92kg | Depois: 83kg</strong></p>
                </div>

                <div class="testimonial">
                    <div class="testimonial-header">
                        <div class="testimonial-avatar">M</div>
                        <div>
                            <h3>Mariana, 28 anos</h3>
                            <div class="stars">★ ★ ★ ★ ★</div>
                        </div>
                    </div>
                    <p>Depois da gravidez estava com dificuldade para perder peso. As receitas e dicas do e-book me ajudaram a perder 6kg sem afetar minha amamentação. Meu marido também adotou os hábitos e já
                        perdeu 5kg!"</p>
                    <p><strong>Antes: 68kg | Depois: 62kg</strong></p>
                </div>
            </div>

            <div class="center">
                <a href="" class="cta-button">QUERO TER RESULTADOS COMO ESTES!</a>
            </div>
        </section>

        <section class="section">
            <h2 class="center">🎁 Bônus Exclusivos</h2>
            <p class="center">(Disponíveis apenas durante esta oferta especial)</p>

            <div class="bonuses">
                <div class="bonus-item">
                    <div class="bonus-icon"><i class="fas fa-shopping-cart"></i></div>
                    <h3>Lista de Compras Inteligente</h3>
                    <p>✔ Alimentos que aceleram o metabolismo</p>
                    <p>✔ Onde comprar com melhor custo-benefício</p>
                    <p>✔ Versão vegetariana inclusa</p>
                </div>

                <div class="bonus-item">
                    <div class="bonus-icon"><i class="fas fa-utensils"></i></div>
                    <h3>Cardápio Semanal Pronto</h3>
                    <p>✔ 4 semanas de refeições planejadas</p>
                    <p>✔ Opções rápida para dias corridos</p>
                    <p>✔ Versão para famílias inclusa</p>
                </div>

                <div class="bonus-item">
                    <div class="bonus-icon"><i class="fas fa-headphones"></i></div>
                    <h3>Áudios de Meditação Guiada</h3>
                    <p>✔ Redução do estresse e ansiedade</p>
                    <p>✔ Controle da compulsão alimentar</p>
                    <p>✔ Melhora na qualidade do sono</p>
                </div>
            </div>

            <div class="center">
                <a href="" class="cta-button">QUERO GARANTIR MEUS BÔNUS!</a>
            </div>
        </section>

        <section class="section section-alt">
            <div class="guarantee">
                <div class="guarantee-number">7</div>
                <h2>Garantia Incondicional de 7 Dias</h2>
                <p>Teste nosso método por 7 dias completos. Se por qualquer motivo você não estiver satisfeito, devolvemos 100% do seu dinheiro sem questionamentos. Sem letras miúdas, sem pegadinhas.</p>
                <p><strong>✔ Você não assume nenhum risco!</strong></p>
            </div>
        </section>

        <section class="section">
            <h2 class="center">❓ Perguntas Frequentes</h2>

            <div class="faq-item">
                <h3>1. Como receberei o e-book após a compra?</h3>
                <p>Imediatamente após a confirmação do pagamento, você receberá um e-mail com o link para download do e-book em PDF e todos os bônus. O processo é automático e você pode acessar o material em
                    qualquer dispositivo.</p>
            </div>

            <div class="faq-item">
                <h3>2. Preciso seguir dietas restritivas com esse método?</h3>
                <p>Não! Nosso foco é na reeducação alimentar e em mudanças sustentáveis. Você aprenderá a fazer escolhas mais inteligentes sem precisar cortar completamente os alimentos que ama. O equilíbrio é a
                    chave.</p>
            </div>

            <div class="faq-item">
                <h3>3. Quanto tempo leva para ver resultados?</h3>
                <p>A maioria dos nossos alunos começa a perceber diferenças já na primeira semana (mais energia, menos inchaço). A perda de peso significativa geralmente ocorre a partir da segunda/terceira semana,
                    variando conforme o metabolismo de cada pessoa.</p>
            </div>

            <div class="faq-item">
                <h3>4. Posso usar o método se tiver problemas de saúde?</h3>
                <p>O método é 100% natural e baseado em alimentos, portanto seguro para a maioria das pessoas. Porém, se você tem condições específicas (diabetes, hipertensão, etc.), recomendamos consultar seu
                    médico antes de iniciar qualquer mudança alimentar.</p>
            </div>

            <div class="faq-item">
                <h3>5. Como funciona a garantia de 7 dias?</h3>
                <p>Se dentro de 7 dias após a compra você achar que o conteúdo não atendeu suas expectativas, basta nos enviar um e-mail que devolveremos todo seu dinheiro, sem burocracia. Você nem precisa
                    justificar sua decisão.</p>
            </div>
        </section>

        <section class="section">
            <div class="offer">
                <h2>⚠️ Oferta por Tempo Limitado!</h2>
                <p>Adquira agora e receba todos os bônus exclusivos</p>

                <div class="countdown" id="countdown">
                    <div class="countdown-item">
                        <div class="countdown-number" id="hours">24</div>
                        <div>Horas</div>
                    </div>
                    <div class="countdown-item">
                        <div class="countdown-number" id="minutes">00</div>
                        <div>Minutos</div>
                    </div>
                    <div class="countdown-item">
                        <div class="countdown-number" id="seconds">00</div>
                        <div>Segundos</div>
                    </div>
                </div>

                <div class="price">
                    <span class="old-price">R$ 97,00</span>
                    <span class="new-price">R$ 29,90</span>
                </div>

                <div class="features">
                    <div class="feature-item"><span class="checkmark">✔</span> E-book completo "Emagrecimento Natural" (PDF)</div>
                    <div class="feature-item"><span class="checkmark">✔</span> Lista de Compras Inteligente (bônus)</div>
                    <div class="feature-item"><span class="checkmark">✔</span> Cardápio Semanal Pronto (bônus)</div>
                    <div class="feature-item"><span class="checkmark">✔</span> Áudios de Meditação Guiada (bônus)</div>
                    <div class="feature-item"><span class="checkmark">✔</span> Acesso Imediato e Vitalício</div>
                    <div class="feature-item"><span class="checkmark">✔</span> Garantia de 7 Dias</div>
                </div>

                <a href="" class="cta-button pulse">SIM, QUERO EMAGRECER AGORA! 🚀</a>

                <div class="payment-badges">
                    <div class="payment-badge"><i class="fas fa-lock"></i> Pagamento Seguro</div>
                    <div class="payment-badge"><i class="fas fa-shield-alt"></i> Dados Protegidos</div>
                    <div class="payment-badge"><i class="fas fa-truck"></i> Entrega Imediata</div>
                </div>

                <p>⏰ Essa oferta pode encerrar a qualquer momento. Não perca essa chance!</p>
            </div>
        </section>
    </div>

    <footer>
        <div class="container">
            <p>💚 Transforme seu corpo e sua saúde com métodos naturais. Sua nova vida começa agora!</p>
            <p>© 2023 Emagrecimento Natural. Todos os direitos reservados.</p>
            <p>Este produto não substitui o parecer médico profissional. Sempre consulte um médico antes de iniciar qualquer programa de emagrecimento.</p>
            <div class="footer-links">
                <a href="#">Termos de Uso</a> | <a href="#">Política de Privacidade</a>
            </div>
        </div>
    </footer>
    <script>
        // Countdown Timer
        function updateCountdown() {
            const now = new Date();
            const target = new Date();
            target.setHours(24, 0, 0, 0); // Set target to tomorrow midnight

            if (now > target) {
                target.setDate(target.getDate() + 1); // Move to next day if already past today's midnight
            }

            const diff = target - now;

            const hours = Math.floor(diff / (1000 * 60 * 60));
            const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((diff % (1000 * 60)) / 1000);

            document.getElementById('hours').textContent = hours.toString().padStart(2, '0');
            document.getElementById('minutes').textContent = minutes.toString().padStart(2, '0');
            document.getElementById('seconds').textContent = seconds.toString().padStart(2, '0');
        }

        // Initialize countdown and update every second
        updateCountdown();
        setInterval(updateCountdown, 1000);

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();

                const targetId = this.getAttribute('href');
                if (targetId === '#') return;

                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    targetElement.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
        // Add animation to elements when they come into view
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = 1;
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);
        // Observe elements for animation
        document.querySelectorAll('.benefit-item, .result-item, .testimonial, .bonus-item').forEach(item => {
            item.style.opacity = 0;
            item.style.transform = 'translateY(20px)';
            item.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(item);
        });
    </script>
</body>

</html>

