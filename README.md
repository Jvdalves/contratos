<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proposta de Parceria Estratégica - João Alves</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', 'Segoe UI', system-ui, -apple-system, sans-serif;
            line-height: 1.6;
            color: #1a1a1a;
            background: #f8fafc;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            min-height: 100vh;
            box-shadow: 0 0 50px rgba(0,0,0,0.05);
        }
        
        .header {
            background: linear-gradient(135deg, #1e293b 0%, #334155 100%);
            color: white;
            padding: 60px 50px;
            position: relative;
        }
        
        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #3b82f6, #8b5cf6, #06b6d4);
        }
        
        .header h1 {
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 12px;
            letter-spacing: -0.02em;
        }
        
        .header .subtitle {
            font-size: 1.4rem;
            opacity: 0.9;
            font-weight: 300;
            margin-bottom: 30px;
        }
        
        .client-info {
            display: flex;
            gap: 40px;
            font-size: 1rem;
            opacity: 0.95;
        }
        
        .client-info div {
            display: flex;
            flex-direction: column;
            gap: 4px;
        }
        
        .client-info .label {
            font-size: 0.85rem;
            opacity: 0.7;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        
        .client-info .value {
            font-weight: 500;
        }
        
        .content {
            padding: 60px 50px;
        }
        
        .section {
            margin-bottom: 60px;
        }
        
        .section-header {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 30px;
            padding-bottom: 15px;
            border-bottom: 1px solid #e2e8f0;
        }
        
        .section-number {
            background: #3b82f6;
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
            font-size: 1.1rem;
        }
        
        .section h2 {
            color: #1e293b;
            font-size: 1.75rem;
            font-weight: 600;
            margin: 0;
        }
        
        .section p {
            color: #475569;
            font-size: 1.1rem;
            margin-bottom: 25px;
        }
        
        .challenge-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 25px 0;
        }
        
        .challenge-item {
            background: #f8fafc;
            border: 1px solid #e2e8f0;
            padding: 25px;
            border-radius: 8px;
            transition: all 0.2s ease;
        }
        
        .challenge-item:hover {
            border-color: #3b82f6;
            background: #f0f9ff;
        }
        
        .challenge-item h3 {
            color: #1e293b;
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 8px;
        }
        
        .challenge-item p {
            color: #64748b;
            margin: 0;
            font-size: 1rem;
        }
        
        .opportunity-box {
            background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
            border: 1px solid #0ea5e9;
            padding: 25px;
            border-radius: 8px;
            margin-top: 25px;
        }
        
        .opportunity-box strong {
            color: #0c4a6e;
        }
        
        .solution-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin: 30px 0;
        }
        
        .solution-item {
            background: #ffffff;
            border: 1px solid #e2e8f0;
            padding: 30px;
            border-radius: 8px;
        }
        
        .solution-item h3 {
            color: #1e293b;
            font-size: 1.3rem;
            font-weight: 600;
            margin-bottom: 20px;
        }
        
        .solution-item ul {
            list-style: none;
            padding: 0;
            margin-bottom: 20px;
        }
        
        .solution-item li {
            padding: 8px 0;
            color: #475569;
            position: relative;
            padding-left: 25px;
        }
        
        .solution-item li::before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #10b981;
            font-weight: 600;
        }
        
        .meta-box {
            background: linear-gradient(135deg, #ecfdf5 0%, #d1fae5 100%);
            border: 1px solid #10b981;
            padding: 15px;
            border-radius: 6px;
            text-align: center;
        }
        
        .meta-box strong {
            color: #065f46;
        }
        
        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 15px;
            margin: 25px 0;
        }
        
        .benefit-item {
            background: #ffffff;
            border: 1px solid #e2e8f0;
            padding: 18px;
            border-radius: 6px;
            display: flex;
            align-items: flex-start;
            gap: 12px;
            transition: all 0.2s ease;
        }
        
        .benefit-item:hover {
            border-color: #10b981;
            background: #f0fdf4;
        }
        
        .benefit-item::before {
            content: "✓";
            color: #10b981;
            font-weight: 600;
            font-size: 1.1rem;
            margin-top: 2px;
            flex-shrink: 0;
        }
        
        .benefit-item span {
            color: #374151;
            font-size: 0.95rem;
        }
        
        .differentials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .differential-item {
            background: #ffffff;
            border: 1px solid #e2e8f0;
            padding: 25px;
            border-radius: 8px;
            text-align: left;
            transition: all 0.2s ease;
        }
        
        .differential-item:hover {
            border-color: #3b82f6;
            background: #f8fafc;
        }
        
        .differential-item strong {
            color: #1e293b;
            font-size: 1.1rem;
            display: block;
            margin-bottom: 8px;
        }
        
        .differential-item p {
            color: #64748b;
            margin: 0;
            font-size: 0.9rem;
        }
        
        .pricing-section {
            background: #f8fafc;
            border: 1px solid #e2e8f0;
            border-radius: 12px;
            padding: 35px;
            margin: 30px 0;
        }
        
        .pricing-table {
            background: white;
            border-radius: 8px;
            border: 1px solid #e2e8f0;
            overflow: hidden;
            margin: 20px 0;
        }
        
        .pricing-table table {
            width: 100%;
            border-collapse: collapse;
        }
        
        .pricing-table th {
            background: #f1f5f9;
            color: #1e293b;
            padding: 20px;
            text-align: left;
            font-weight: 600;
            font-size: 0.95rem;
            border-bottom: 1px solid #e2e8f0;
        }
        
        .pricing-table td {
            padding: 20px;
            border-bottom: 1px solid #f1f5f9;
            vertical-align: top;
        }
        
        .pricing-table tr:hover {
            background: #f8fafc;
        }
        
        .price {
            font-size: 1.4rem;
            font-weight: 700;
            color: #dc2626;
        }
        
        .advantage-box {
            background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
            border: 1px solid #3b82f6;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            margin: 25px 0;
        }
        
        .advantage-box strong {
            color: #1e40af;
        }
        
        .investment-note {
            background: #fffbeb;
            border: 1px solid #f59e0b;
            padding: 25px;
            border-radius: 8px;
            margin: 25px 0;
        }
        
        .investment-note h4 {
            color: #92400e;
            margin-bottom: 15px;
            font-size: 1.1rem;
        }
        
        .investment-note ul {
            list-style: none;
            padding: 0;
        }
        
        .investment-note li {
            padding: 5px 0;
            color: #78350f;
            position: relative;
            padding-left: 25px;
        }
        
        .investment-note li::before {
            content: "•";
            position: absolute;
            left: 0;
            color: #f59e0b;
            font-weight: 600;
        }
        
        .timeline-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .timeline-item {
            background: white;
            border: 1px solid #e2e8f0;
            padding: 25px;
            border-radius: 8px;
            text-align: center;
            position: relative;
            transition: all 0.2s ease;
        }
        
        .timeline-item:hover {
            border-color: #06b6d4;
            background: #f0fdfa;
        }
        
        .timeline-item::before {
            content: "";
            position: absolute;
            top: -8px;
            left: 50%;
            transform: translateX(-50%);
            width: 16px;
            height: 16px;
            background: #06b6d4;
            border-radius: 50%;
            border: 3px solid white;
        }
        
        .timeline-item h4 {
            color: #1e293b;
            font-size: 1.1rem;
            font-weight: 600;
            margin-bottom: 10px;
        }
        
        .timeline-item p {
            color: #64748b;
            margin: 0;
            font-size: 0.9rem;
        }
        
        .closing-section {
            background: linear-gradient(135deg, #1e293b 0%, #334155 100%);
            color: white;
            padding: 50px;
            border-radius: 12px;
            text-align: center;
            margin-top: 40px;
        }
        
        .closing-section h2 {
            font-size: 1.8rem;
            font-weight: 600;
            margin-bottom: 20px;
            color: white;
        }
        
        .closing-section p {
            font-size: 1.2rem;
            line-height: 1.7;
            opacity: 0.95;
            margin: 0;
        }
        
        @media (max-width: 768px) {
            .header, .content {
                padding: 40px 25px;
            }
            
            .header h1 {
                font-size: 2.2rem;
            }
            
            .client-info {
                flex-direction: column;
                gap: 15px;
            }
            
            .solution-grid {
                grid-template-columns: 1fr;
                gap: 20px;
            }
            
            .section {
                margin-bottom: 40px;
            }
            
            .challenge-grid, .benefits-grid, .differentials-grid {
                grid-template-columns: 1fr;
            }
            
            .pricing-table {
                overflow-x: auto;
            }
            
            .pricing-table table {
                min-width: 600px;
            }
        }
        
        @media (max-width: 480px) {
            .header, .content {
                padding: 25px 15px;
            }
            
            .header h1 {
                font-size: 1.8rem;
            }
            
            .header .subtitle {
                font-size: 1.2rem;
            }
            
            .section-number {
                width: 32px;
                height: 32px;
                font-size: 0.9rem;
            }
            
            .section h2 {
                font-size: 1.4rem;
            }
            
            .pricing-section, .investment-note, .opportunity-box {
                padding: 20px;
            }
            
            .pricing-table th, .pricing-table td {
                padding: 12px 8px;
                font-size: 0.85rem;
            }
            
            .price {
                font-size: 1.2rem;
            }
            
            .closing-section {
                padding: 35px 25px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Proposta de Parceria Estratégica</h1>
            <div class="subtitle">Marketing e Branding</div>
            <div class="client-info">
                <div>
                    <div class="label">Apresentada por</div>
                    <div class="value">Diferenciais Marketing</div>
                </div>
                <div>
                    <div class="label">Cliente</div>
                    <div class="value">João Bosco (Escritório + Bossacf Bistrô + São Carinpudas)</div>
                </div>
            </div>
        </div>
        
        <div class="content">
            <div class="section">
                <div class="section-header">
                    <div class="section-number">01</div>
                    <h2>O Desafio Identificado</h2>
                </div>
                <p>Três negócios com grande potencial precisam de uma estratégia integrada para maximizar seu crescimento e consolidação no mercado.</p>
                
                <div class="challenge-grid">
                    <div class="challenge-item">
                        <h3>Escritório Jurídico</h3>
                        <p>Captar leads qualificados e humanizar a marca para gerar mais conversões</p>
                    </div>
                    <div class="challenge-item">
                        <h3>Bossacf Bistrô</h3>
                        <p>Consolidar presença digital para atrair e fidelizar público de alto padrão</p>
                    </div>
                    <div class="challenge-item">
                        <h3>São Carinpudas</h3>
                        <p>Aumentar pedidos via iFood e construir relacionamento duradouro com clientes</p>
                    </div>
                </div>
                
                <div class="opportunity-box">
                    <strong>A oportunidade:</strong> unificar a comunicação dos três CNPJs com identidade consistente e estratégia personalizada para cada público, criando sinergia entre os negócios.
                </div>
            </div>
            
            <div class="section">
                <div class="section-header">
                    <div class="section-number">02</div>
                    <h2>Nossa Solução Estratégica</h2>
                </div>
                
                <div class="solution-grid">
                    <div class="solution-item">
                        <h3>Para o Escritório João Bosco</h3>
                        <ul>
                            <li>3 vídeos semanais (autoridade + humanização)</li>
                            <li>2 criativos de tráfego pago</li>
                            <li>Acompanhamento completo nas redes sociais</li>
                        </ul>
                        <div class="meta-box">
                            <strong>Meta:</strong> 35+ leads qualificados/mês
                        </div>
                    </div>
                    <div class="solution-item">
                        <h3>Para Bossacf Bistrô e São Carinpudas</h3>
                        <p style="margin-bottom: 15px; font-weight: 500;">Cada restaurante recebe:</p>
                        <ul>
                            <li>3 vídeos semanais</li>
                            <li>2 criativos de tráfego pago</li>
                            <li>Catálogo digital completo</li>
                            <li>Configuração e otimização do iFood</li>
                        </ul>
                        <div class="meta-box">
                            <strong>Meta:</strong> 250+ leads/pedidos por estabelecimento
                        </div>
                    </div>
                </div>
                
                <h3 style="margin: 40px 0 20px 0; color: #1e293b; font-size: 1.3rem;">Benefícios Extras Inclusos</h3>
                <div class="benefits-grid">
                    <div class="benefit-item"><span>Identidade visual e verbal completa para os 3 CNPJs</span></div>
                    <div class="benefit-item"><span>Consultoria estratégica contínua</span></div>
                    <div class="benefit-item"><span>Time dedicado: profissional adicional para garantir qualidade</span></div>
                    <div class="benefit-item"><span>Treinamento da equipe para atendimento digital</span></div>
                    <div class="benefit-item"><span>Relatórios mensais de performance com otimização constante</span></div>
                    <div class="benefit-item"><span>Backup garantido: nunca haverá atraso por sobrecarga</span></div>
                    <div class="benefit-item"><span>Bônus por metas atingidas: conteúdos extras sem custo</span></div>
                    <div class="benefit-item"><span>Consultoria de expansão: análise de cardápio e estratégias</span></div>
                </div>
            </div>
            
            <div class="section">
                <div class="section-header">
                    <div class="section-number">03</div>
                    <h2>Por Que Escolher a Diferenciais</h2>
                </div>
                
                <div class="differentials-grid">
                    <div class="differential-item">
                        <strong>Gestor de tráfego especialista</strong>
                        <p>Experiência comprovada em campanhas de alta performance e otimização de ROI</p>
                    </div>
                    <div class="differential-item">
                        <strong>Time dedicado</strong>
                        <p>Equipe especializada para elevar a qualidade das entregas e garantir prazos</p>
                    </div>
                    <div class="differential-item">
                        <strong>Proximidade real</strong>
                        <p>Acompanhamento direto e personalizado com ajustes rápidos quando necessário</p>
                    </div>
                    <div class="differential-item">
                        <strong>Visão estratégica</strong>
                        <p>Não apenas execução, mas planejamento integral de crescimento sustentável</p>
                    </div>
                    <div class="differential-item">
                        <strong>Criatividade diferenciada</strong>
                        <p>Conteúdo autêntico e impactante que marca presença e gera conversões</p>
                    </div>
                    <div class="differential-item">
                        <strong>Transparência total</strong>
                        <p>Relatórios detalhados e claros que demonstram ROI real dos investimentos</p>
                    </div>
                </div>
            </div>
            
            <div class="section">
                <div class="section-header">
                    <div class="section-number">04</div>
                    <h2>Modelo de Investimento Progressivo</h2>
                </div>
                
                <div class="pricing-section">
                    <div class="pricing-table">
                        <table>
                            <thead>
                                <tr>
                                    <th>Etapa</th>
                                    <th>Condição para Avanço</th>
                                    <th>Investimento</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td><strong>Meta 1</strong></td>
                                    <td>Estruturas de branding + iFood otimizado + 35 leads escritório OU 250 pedidos restaurantes</td>
                                    <td><span class="price">R$ 2.500/mês</span></td>
                                </tr>
                                <tr>
                                    <td><strong>Meta 2</strong></td>
                                    <td>100 leads qualificados escritório + 700 pedidos iFood</td>
                                    <td><span class="price">R$ 5.500/mês</span></td>
                                </tr>
                                <tr>
                                    <td><strong>Meta Final</strong></td>
                                    <td>Fluxo consolidado e recorrente</td>
                                    <td><span class="price">R$ 7.000/mês</span></td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                    
                    <div class="advantage-box">
                        <strong>Vantagem competitiva:</strong> você investe mais apenas quando os resultados estão comprovados e gerando retorno real.
                    </div>
                    
                    <div class="investment-note">
                        <h4>Investimentos Recomendados (não obrigatórios inicialmente)</h4>
                        <ul>
                            <li><strong>Tráfego pago:</strong> R$ 1.000/mês por negócio (total R$ 3.000/mês)</li>
                            <li><strong>Foco inicial:</strong> Pelo menos 1 CNPJ para otimização de recursos</li>
                            <li><strong>Pagamento:</strong> Valores direcionados diretamente às plataformas (Meta, Google, etc.)</li>
                        </ul>
                    </div>
                </div>
            </div>
            
            <div class="section">
                <div class="section-header">
                    <div class="section-number">05</div>
                    <h2>Timeline de Resultados</h2>
                </div>
                
                <div class="timeline-container">
                    <div class="timeline-item">
                        <h4>Primeiros 30 dias</h4>
                        <p>Criativos prontos, campanhas ativas e iFood totalmente configurado e otimizado</p>
                    </div>
                    <div class="timeline-item">
                        <h4>60 dias</h4>
                        <p>Primeiros resultados mensuráveis com relatórios detalhados de performance</p>
                    </div>
                    <div class="timeline-item">
                        <h4>A partir dos 60 dias</h4>
                        <p>Avaliação completa e possível escalonamento para próxima meta</p>
                    </div>
                </div>
            </div>
            
            <div class="closing-section">
                <h2>Uma Parceria para Crescimento Sustentável</h2>
                <p>Esta proposta foi desenvolvida para gerar resultados reais e mensuráveis. Mais do que um fornecedor de marketing, você terá um parceiro estratégico focado no crescimento sustentável dos seus três negócios, com total transparência e compromisso com a excelência.</p>
            </div>
        </div>
    </div>
</body>
</html>
