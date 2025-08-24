<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Johana Quintana Blas - QA Specialist & AI Expert</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.4;
            color: #333;
            background: #f0f0f0;
            font-size: 14px;
        }

        .cv-container {
            max-width: 210mm;
            margin: 20px auto;
            background: white;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
            min-height: 297mm;
        }

        .header {
            background: linear-gradient(45deg, #2c3e50, #3498db, #16a085);
            color: white;
            padding: 30px;
            text-align: center;
        }

        .name {
            font-size: 28px;
            font-weight: bold;
            margin-bottom: 8px;
        }

        .title {
            font-size: 16px;
            margin-bottom: 15px;
            opacity: 0.9;
        }

        .summary {
            font-size: 14px;
            line-height: 1.5;
            max-width: 600px;
            margin: 0 auto;
        }

        .main-content {
            display: flex;
            min-height: calc(297mm - 140px);
        }

        .sidebar {
            width: 35%;
            background: #f8f9fa;
            padding: 25px 20px;
        }

        .content {
            width: 65%;
            padding: 25px 20px;
        }

        .section-title {
            font-size: 18px;
            font-weight: bold;
            color: #2c3e50;
            margin-bottom: 15px;
            border-bottom: 2px solid #16a085;
            padding-bottom: 5px;
        }

        .sidebar .section-title {
            font-size: 16px;
            margin-bottom: 12px;
        }

        .contact-info {
            background: white;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 20px;
            border-left: 4px solid #16a085;
        }

        .contact-item {
            margin: 8px 0;
            font-size: 13px;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 8px;
            margin-top: 10px;
        }

        .tech-item {
            background: linear-gradient(45deg, #16a085, #3498db);
            color: white;
            padding: 8px;
            text-align: center;
            border-radius: 6px;
            font-size: 12px;
            font-weight: 500;
        }

        .education-item, .cert-item {
            background: white;
            padding: 12px;
            margin: 8px 0;
            border-radius: 6px;
            border-left: 3px solid #e74c3c;
            font-size: 13px;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin: 20px 0;
        }

        .stat-card {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            border-left: 4px solid #3498db;
        }

        .stat-number {
            font-size: 24px;
            font-weight: bold;
            color: #3498db;
        }

        .stat-label {
            color: #666;
            font-size: 12px;
        }

        .highlight {
            background: linear-gradient(120deg, rgba(22,160,133,0.1), rgba(52,152,219,0.1));
            padding: 15px;
            border-radius: 8px;
            margin: 15px 0;
            border-left: 4px solid #16a085;
        }

        .highlight h4 {
            color: #2c3e50;
            margin-bottom: 8px;
            font-size: 16px;
        }

        .highlight p {
            margin: 5px 0;
            font-size: 13px;
        }

        .experience-item {
            background: #f8f9fa;
            padding: 18px;
            margin-bottom: 18px;
            border-radius: 8px;
            border-left: 4px solid #3498db;
        }

        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 12px;
        }

        .job-title {
            font-size: 16px;
            font-weight: bold;
            color: #2c3e50;
        }

        .company {
            font-size: 14px;
            color: #3498db;
            font-weight: 500;
        }

        .duration {
            color: #666;
            font-size: 12px;
            background: #e9ecef;
            padding: 4px 8px;
            border-radius: 12px;
        }

        .achievements {
            list-style: none;
            padding: 0;
        }

        .achievements li {
            padding: 4px 0;
            padding-left: 15px;
            position: relative;
            font-size: 13px;
        }

        .achievements li::before {
            content: '→';
            position: absolute;
            left: 0;
            color: #3498db;
            font-weight: bold;
        }

        .skill-category {
            margin-bottom: 20px;
        }

        .skill-category h4 {
            color: #2c3e50;
            font-size: 14px;
            margin-bottom: 8px;
        }

        .skill-item {
            background: white;
            padding: 8px 12px;
            margin: 4px 0;
            border-radius: 15px;
            border-left: 3px solid #16a085;
            font-size: 12px;
        }

        .project-section {
            border-left: 5px solid #16a085;
            background: linear-gradient(135deg, rgba(22,160,133,0.1) 0%, rgba(52,152,219,0.1) 100%);
            margin-bottom: 20px;
        }

        .podcast-section {
            border-left: 5px solid #e91e63;
            background: linear-gradient(135deg, rgba(233,30,99,0.1) 0%, rgba(255,193,7,0.1) 100%);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 12px;
            margin: 15px 0;
        }

        .service-card {
            background: white;
            padding: 12px;
            border-radius: 6px;
            border-left: 3px solid #3498db;
        }

        .service-card h5 {
            color: #2c3e50;
            margin-bottom: 6px;
            font-size: 13px;
        }

        .service-card ul {
            list-style: none;
            padding: 0;
        }

        .service-card li {
            padding: 2px 0;
            font-size: 11px;
        }

        .philosophy-box {
            background: #4a148c;
            color: white;
            padding: 12px;
            border-radius: 6px;
            text-align: center;
            margin: 10px 0;
        }

        .philosophy-box h4 {
            color: #ffc107;
            margin-bottom: 5px;
        }

        .contact-footer {
            background: #2c3e50;
            color: white;
            padding: 8px;
            border-radius: 6px;
            text-align: center;
            margin-top: 10px;
            font-size: 12px;
        }

        .download-btn {
            position: fixed;
            top: 20px;
            right: 20px;
            background: #16a085;
            color: white;
            border: none;
            padding: 12px 20px;
            border-radius: 25px;
            cursor: pointer;
            font-size: 14px;
            box-shadow: 0 4px 12px rgba(22, 160, 133, 0.3);
            z-index: 1000;
        }

        .download-btn:hover {
            background: #148f77;
        }

        @media print {
            body { 
                background: white; 
                font-size: 12px;
            }
            .cv-container { 
                margin: 0; 
                box-shadow: none; 
                max-width: none;
            }
            .download-btn { 
                display: none; 
            }
            .main-content {
                min-height: auto;
            }
            .experience-item {
                break-inside: avoid;
                margin-bottom: 12px;
            }
            .project-section {
                break-inside: avoid;
            }
        }

        @media (max-width: 768px) {
            .cv-container {
                margin: 10px;
                max-width: none;
            }
            .main-content {
                flex-direction: column;
            }
            .sidebar, .content {
                width: 100%;
            }
            .stats {
                grid-template-columns: repeat(2, 1fr);
            }
            .services-grid {
                grid-template-columns: 1fr;
            }
            .job-header {
                flex-direction: column;
                gap: 8px;
            }
        }
    </style>
</head>
<body>
    <div class="cv-container">
        <header class="header">
            <h1 class="name">Johana Atenas Quintana Blas</h1>
            <div class="title">QA Specialist | AI Expert | Agile Leader | Entrepreneur</div>
            <p class="summary">
                Especialista en calidad de software con experiencia sólida en el sector financiero y asegurador. 
                Emprendedora social enfocada en desarrollar nuevos talentos QA. A partir de enero 2025, impulsa 
                AI Testing Training & Services y el Podcast QA-blando, democratizando el conocimiento en calidad 
                de software con estándares internacionales.
            </p>
        </header>

        <div class="main-content">
            <aside class="sidebar">
                <div class="contact-info">
                    <h3 style="color: #2c3e50; margin-bottom: 10px; font-size: 16px;">Contacto</h3>
                    <div class="contact-item">
                        📧 quintanablasjohanaatenas@gmail.com
                    </div>
                    <div class="contact-item">
                        📱 +51 980 565 944
                    </div>
                    <div class="contact-item">
                        📍 Lima, Perú
                    </div>
                </div>

                <div class="section">
                    <h3 class="section-title">Tecnologías</h3>
                    <div class="tech-grid">
                        <div class="tech-item">Python</div>
                        <div class="tech-item">Java</div>
                        <div class="tech-item">COBOL</div>
                        <div class="tech-item">Selenium</div>
                        <div class="tech-item">SQL</div>
                        <div class="tech-item">DB2</div>
                        <div class="tech-item">Oracle</div>
                        <div class="tech-item">Jira</div>
                        <div class="tech-item">Jenkins</div>
                        <div class="tech-item">MongoDB</div>
                        <div class="tech-item">Postman</div>
                        <div class="tech-item">SonarCloud</div>
                    </div>
                </div>

                <div class="section">
                    <h3 class="section-title">Educación</h3>
                    <div class="education-item">
                        <strong>Especialización en IA</strong><br>
                        <small>USIL (2024-2025)</small>
                    </div>
                    <div class="education-item">
                        <strong>Bachiller en Ingeniería</strong><br>
                        <small>UPCI (2007-2012)</small>
                    </div>
                    <div class="education-item">
                        <strong>Administrador de Redes</strong><br>
                        <small>TECSUP (2012)</small>
                    </div>
                </div>

                <div class="section">
                    <h3 class="section-title">Certificaciones</h3>
                    <div class="cert-item">GAIPC™ - Generative AI Professional</div>
                    <div class="cert-item">CPEFPC™ - Prompt Engineering</div>
                    <div class="cert-item">ISTQB CTFL 4.0</div>
                    <div class="cert-item">Scrum Master SMPC®</div>
                    <div class="cert-item">AWS IA Generativa</div>
                </div>
            </aside>

            <main class="content">
                <div class="stats">
                    <div class="stat-card">
                        <div class="stat-number">9+</div>
                        <div class="stat-label">Años Experiencia</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">30%</div>
                        <div class="stat-label">Mejora en Eficiencia</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">2</div>
                        <div class="stat-label">Emprendimientos</div>
                    </div>
                </div>

                <div class="highlight">
                    <h4>🚀 Especialidades Clave & Nuevos Proyectos 2025</h4>
                    <p><strong>IA Generativa:</strong> Desarrollo de soluciones para detección de anomalías y automatización</p>
                    <p><strong>Liderazgo Ágil:</strong> Coordinación de equipos multidisciplinarios</p>
                    <p><strong>Emprendimiento en Desarrollo:</strong> Nuevos talentos QA y democratización del conocimiento</p>
                </div>

                <div class="section">
                    <h2 class="section-title">🌟 Nuevas Iniciativas 2025</h2>
                    
                    <div class="experience-item project-section">
                        <div class="job-header">
                            <div>
                                <div class="job-title">🏢 AI Testing Training & Services</div>
                                <div class="company" style="color: #16a085;">Fundadora & Consultora Principal</div>
                            </div>
                            <div class="duration">Ene 2025 - Presente</div>
                        </div>
                        
                        <div style="background: white; padding: 10px; border-radius: 6px; margin: 10px 0; text-align: center; border-left: 3px solid #16a085;">
                            <em style="color: #2c3e50; font-size: 14px;">"Transformamos profesionales IT en Quality Engineers certificados internacionalmente"</em>
                        </div>
                        
                        <div class="services-grid">
                            <div class="service-card">
                                <h5>📚 CAPACITACIÓN & CERTIFICACIÓN</h5>
                                <ul>
                                    <li>✅ Fundamentos del Analista de Calidad</li>
                                    <li>✅ Capacitación basada en ISTQB</li>
                                    <li>✅ Testing Manual y Automatizado</li>
                                    <li>✅ Mentoría personalizada</li>
                                </ul>
                            </div>
                            <div class="service-card">
                                <h5>⚙️ SERVICIOS DE CALIDAD</h5>
                                <ul>
                                    <li>✅ Testing web y móvil</li>
                                    <li>✅ Automatización de pruebas</li>
                                    <li>✅ Auditorías de calidad</li>
                                    <li>✅ Testing de APIs</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <div class="experience-item podcast-section">
                        <div class="job-header">
                            <div>
                                <div class="job-title">🎙️ Podcast QA-blando</div>
                                <div class="company" style="color: #e91e63;">Host & Creadora de Contenido</div>
                            </div>
                            <div class="duration">Ene 2025 - Presente</div>
                        </div>
                        
                        <div class="philosophy-box">
                            <h4>"Serios pero no tan serios"</h4>
                            <p style="margin: 0; font-size: 12px;">Democratizando el conocimiento en calidad de software para la comunidad hispanohablante</p>
                        </div>
                        
                        <div class="services-grid">
                            <div class="service-card" style="border-left-color: #e91e63;">
                                <h5>🎤 Contenido Educativo</h5>
                                <ul>
                                    <li>📻 Tips prácticos de QA</li>
                                    <li>📻 Entrevistas a expertos</li>
                                    <li>📻 Casos de estudio reales</li>
                                    <li>📻 Tendencias en testing</li>
                                </ul>
                            </div>
                            <div class="service-card" style="border-left-color: #ffc107;">
                                <h5>🌟 Impacto Social</h5>
                                <ul>
                                    <li>🌍 Acceso gratuito al conocimiento</li>
                                    <li>🌍 Comunidad QA en español</li>
                                    <li>🌍 Mentoría a nuevos talentos</li>
                                    <li>🌍 Networking profesional</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="section">
                    <h2 class="section-title">Competencias Principales</h2>
                    
                    <div class="skill-category">
                        <h4>🔍 Aseguramiento y Control de Calidad</h4>
                        <div class="skill-item">Análisis y estrategias de prueba personalizadas</div>
                        <div class="skill-item">Supervisión de ciclos completos de testing</div>
                        <div class="skill-item">Optimización de procesos y reducción de tiempos</div>
                        <div class="skill-item">Evaluación CMMI3 y estándares de calidad</div>
                    </div>

                    <div class="skill-category">
                        <h4>🤖 IA Generativa & Automatización</h4>
                        <div class="skill-item">Soluciones basadas en IA para detección de anomalías</div>
                        <div class="skill-item">Automatización de pruebas con técnicas de IA</div>
                        <div class="skill-item">Desarrollo en Python, Java, COBOL y Selenium</div>
                        <div class="skill-item">Gestión de BD: SQL, DB2, Oracle</div>
                    </div>

                    <div class="skill-category">
                        <h4>👥 Liderazgo & Gestión</h4>
                        <div class="skill-item">Coordinación de equipos multidisciplinarios</div>
                        <div class="skill-item">Capacitación en metodologías ágiles</div>
                        <div class="skill-item">Gestión de recursos y presupuestos</div>
                        <div class="skill-item">Herramientas: Jira, Xray, Jenkins, Bitbucket</div>
                    </div>
                </div>

                <div class="section">
                    <h2 class="section-title">Experiencia Profesional Destacada</h2>

                    <div class="experience-item">
                        <div class="job-header">
                            <div>
                                <div class="job-title">Analista Senior de Aseguramiento y Control de Calidad</div>
                                <div class="company">La Positiva Seguros</div>
                            </div>
                            <div class="duration">Oct 2022 - Presente</div>
                        </div>
                        <ul class="achievements">
                            <li><strong>Liderazgo:</strong> Coordinación de equipos de calidad y supervisión de Automatización</li>
                            <li><strong>Optimización:</strong> Reducción del 20% en costos operativos</li>
                            <li><strong>IA Implementada:</strong> Aumento del 30% en velocidad de pruebas</li>
                            <li><strong>Capacitación:</strong> Desarrollo profesional en IA, Jenkins y Selenium</li>
                        </ul>
                    </div>

                    <div class="experience-item">
                        <div class="job-header">
                            <div>
                                <div class="job-title">Analista Funcional QA Senior</div>
                                <div class="company">Indra - Proyecto BBVA</div>
                            </div>
                            <div class="duration">Jul 2021 - Sep 2022</div>
                        </div>
                        <ul class="achievements">
                            <li><strong>Core Transactional:</strong> Aseguramiento en transferencias interbancarias</li>
                            <li><strong>Optimización:</strong> Reducción del 15% en tiempo de ejecución</li>
                            <li><strong>Proyectos Clave:</strong> Participación en Vocalink y liderazgo en Proyecto CIRCULAR</li>
                        </ul>
                    </div>

                    <div class="experience-item">
                        <div class="job-header">
                            <div>
                                <div class="job-title">Analista Técnico Senior</div>
                                <div class="company">Canvia - Proyectos NIUVIZ, CLARO, BBVA</div>
                            </div>
                            <div class="duration">Oct 2018 - May 2021</div>
                        </div>
                        <ul class="achievements">
                            <li><strong>VISANET:</strong> Liderazgo en pruebas de omnicanalidad, innovación y CRM</li>
                            <li><strong>Reducción de Incidentes:</strong> 20% menos incidentes en producción</li>
                            <li><strong>Múltiples Proyectos:</strong> CLARO, BBVA con mejoras significativas</li>
                        </ul>
                    </div>

                    <div class="experience-item">
                        <div class="job-header">
                            <div>
                                <div class="job-title">Roles Previos - Analista Funcional & Developer</div>
                                <div class="company">MDP Consulting, Globokas, Everis, TCS</div>
                            </div>
                            <div class="duration">2014 - 2018</div>
                        </div>
                        <ul class="achievements">
                            <li><strong>Sectores:</strong> Bancario, Telecomunicaciones, Medios de Pago</li>
                            <li><strong>Especialización:</strong> COBOL, SOA, Integración de Servicios</li>
                            <li><strong>Metodologías:</strong> Ágil, Cascada, PAR</li>
                            <li><strong>Estándares:</strong> CMMI3 y CMMI5, mejora continua</li>
                        </ul>
                    </div>
                </div>
                
                <div class="contact-footer">
                    <strong>📋 PROYECTOS Y CAPACITACIONES</strong><br>
                    📧 E-mail: aitestingservicesperu@gmail.com<br>
                    📞 Teléfono: +51 992 097 896
                </div>
            </main>
        </div>
    </div>

    <button class="download-btn" onclick="window.print()">
        📄 Descargar PDF
    </button>

    <script>
        // Optimización para impresión
        window.addEventListener('beforeprint', function() {
            document.body.style.fontSize = '11px';
        });

        window.addEventListener('afterprint', function() {
            document.body.style.fontSize = '14px';
        });

        // Función para generar PDF
        function generatePDF() {
            // Ajustar estilos para PDF
            const originalStyle = document.body.style.cssText;
            document.body.style.cssText += 'font-size: 11px !important;';
            
            // Imprimir
            window.print();
            
            // Restaurar estilos
            setTimeout(() => {
                document.body.style.cssText = originalStyle;
            }, 1000);
        }

        // Optimizar botón
        document.querySelector('.download-btn').onclick = generatePDF;
    </script>
</body>
</html><!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Johana Quintana Blas - QA Specialist & AI Expert</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.4;
            color: #333;
            background: #f0f0f0;
            font-size: 14px;
        }

        .cv-container {
            max-width: 210mm;
            margin: 20px auto;
            background: white;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
            min-height: 297mm;
        }

        .header {
            background: linear-gradient(45deg, #2c3e50, #3498db, #16a085);
            color: white;
            padding: 30px;
            text-align: center;
        }

        .name {
            font-size: 28px;
            font-weight: bold;
            margin-bottom: 8px;
        }

        .title {
            font-size: 16px;
            margin-bottom: 15px;
            opacity: 0.9;
        }

        .summary {
            font-size: 14px;
            line-height: 1.5;
            max-width: 600px;
            margin: 0 auto;
        }

        .main-content {
            display: flex;
            min-height: calc(297mm - 140px);
        }

        .sidebar {
            width: 35%;
            background: #f8f9fa;
            padding: 25px 20px;
        }

        .content {
            width: 65%;
            padding: 25px 20px;
        }

        .section-title {
            font-size: 18px;
            font-weight: bold;
            color: #2c3e50;
            margin-bottom: 15px;
            border-bottom: 2px solid #16a085;
            padding-bottom: 5px;
        }

        .sidebar .section-title {
            font-size: 16px;
            margin-bottom: 12px;
        }

        .contact-info {
            background: white;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 20px;
            border-left: 4px solid #16a085;
        }

        .contact-item {
            margin: 8px 0;
            font-size: 13px;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 8px;
            margin-top: 10px;
        }

        .tech-item {
            background: linear-gradient(45deg, #16a085, #3498db);
            color: white;
            padding: 8px;
            text-align: center;
            border-radius: 6px;
            font-size: 12px;
            font-weight: 500;
        }

        .education-item, .cert-item {
            background: white;
            padding: 12px;
            margin: 8px 0;
            border-radius: 6px;
            border-left: 3px solid #e74c3c;
            font-size: 13px;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin: 20px 0;
        }

        .stat-card {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            border-left: 4px solid #3498db;
        }

        .stat-number {
            font-size: 24px;
            font-weight: bold;
            color: #3498db;
        }

        .stat-label {
            color: #666;
            font-size: 12px;
        }

        .highlight {
            background: linear-gradient(120deg, rgba(22,160,133,0.1), rgba(52,152,219,0.1));
            padding: 15px;
            border-radius: 8px;
            margin: 15px 0;
            border-left: 4px solid #16a085;
        }

        .highlight h4 {
            color: #2c3e50;
            margin-bottom: 8px;
            font-size: 16px;
        }

        .highlight p {
            margin: 5px 0;
            font-size: 13px;
        }

        .experience-item {
            background: #f8f9fa;
            padding: 18px;
            margin-bottom: 18px;
            border-radius: 8px;
            border-left: 4px solid #3498db;
        }

        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 12px;
        }

        .job-title {
            font-size: 16px;
            font-weight: bold;
            color: #2c3e50;
        }

        .company {
            font-size: 14px;
            color: #3498db;
            font-weight: 500;
        }

        .duration {
            color: #666;
            font-size: 12px;
            background: #e9ecef;
            padding: 4px 8px;
            border-radius: 12px;
        }

        .achievements {
            list-style: none;
            padding: 0;
        }

        .achievements li {
            padding: 4px 0;
            padding-left: 15px;
            position: relative;
            font-size: 13px;
        }

        .achievements li::before {
            content: '→';
            position: absolute;
            left: 0;
            color: #3498db;
            font-weight: bold;
        }

        .skill-category {
            margin-bottom: 20px;
        }

        .skill-category h4 {
            color: #2c3e50;
            font-size: 14px;
            margin-bottom: 8px;
        }

        .skill-item {
            background: white;
            padding: 8px 12px;
            margin: 4px 0;
            border-radius: 15px;
            border-left: 3px solid #16a085;
            font-size: 12px;
        }

        .project-section {
            border-left: 5px solid #16a085;
            background: linear-gradient(135deg, rgba(22,160,133,0.1) 0%, rgba(52,152,219,0.1) 100%);
            margin-bottom: 20px;
        }

        .podcast-section {
            border-left: 5px solid #e91e63;
            background: linear-gradient(135deg, rgba(233,30,99,0.1) 0%, rgba(255,193,7,0.1) 100%);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 12px;
            margin: 15px 0;
        }

        .service-card {
            background: white;
            padding: 12px;
            border-radius: 6px;
            border-left: 3px solid #3498db;
        }

        .service-card h5 {
            color: #2c3e50;
            margin-bottom: 6px;
            font-size: 13px;
        }

        .service-card ul {
            list-style: none;
            padding: 0;
        }

        .service-card li {
            padding: 2px 0;
            font-size: 11px;
        }

        .philosophy-box {
            background: #4a148c;
            color: white;
            padding: 12px;
            border-radius: 6px;
            text-align: center;
            margin: 10px 0;
        }

        .philosophy-box h4 {
            color: #ffc107;
            margin-bottom: 5px;
        }

        .contact-footer {
            background: #2c3e50;
            color: white;
            padding: 8px;
            border-radius: 6px;
            text-align: center;
            margin-top: 10px;
            font-size: 12px;
        }

        .download-btn {
            position: fixed;
            top: 20px;
            right: 20px;
            background: #16a085;
            color: white;
            border: none;
            padding: 12px 20px;
            border-radius: 25px;
            cursor: pointer;
            font-size: 14px;
            box-shadow: 0 4px 12px rgba(22, 160, 133, 0.3);
            z-index: 1000;
        }

        .download-btn:hover {
            background: #148f77;
        }

        @media print {
            body { 
                background: white; 
                font-size: 12px;
            }
            .cv-container { 
                margin: 0; 
                box-shadow: none; 
                max-width: none;
            }
            .download-btn { 
                display: none; 
            }
            .main-content {
                min-height: auto;
            }
            .experience-item {
                break-inside: avoid;
                margin-bottom: 12px;
            }
            .project-section {
                break-inside: avoid;
            }
        }

        @media (max-width: 768px) {
            .cv-container {
                margin: 10px;
                max-width: none;
            }
            .main-content {
                flex-direction: column;
            }
            .sidebar, .content {
                width: 100%;
            }
            .stats {
                grid-template-columns: repeat(2, 1fr);
            }
            .services-grid {
                grid-template-columns: 1fr;
            }
            .job-header {
                flex-direction: column;
                gap: 8px;
            }
        }
    </style>
</head>
<body>
    <div class="cv-container">
        <header class="header">
            <h1 class="name">Johana Atenas Quintana Blas</h1>
            <div class="title">QA Specialist | AI Expert | Agile Leader | Entrepreneur</div>
            <p class="summary">
                Especialista en calidad de software con experiencia sólida en el sector financiero y asegurador. 
                Emprendedora social enfocada en desarrollar nuevos talentos QA. A partir de enero 2025, impulsa 
                AI Testing Training & Services y el Podcast QA-blando, democratizando el conocimiento en calidad 
                de software con estándares internacionales.
            </p>
        </header>

        <div class="main-content">
            <aside class="sidebar">
                <div class="contact-info">
                    <h3 style="color: #2c3e50; margin-bottom: 10px; font-size: 16px;">Contacto</h3>
                    <div class="contact-item">
                        📧 quintanablasjohanaatenas@gmail.com
                    </div>
                    <div class="contact-item">
                        📱 +51 980 565 944
                    </div>
                    <div class="contact-item">
                        📍 Lima, Perú
                    </div>
                </div>

                <div class="section">
                    <h3 class="section-title">Tecnologías</h3>
                    <div class="tech-grid">
                        <div class="tech-item">Python</div>
                        <div class="tech-item">Java</div>
                        <div class="tech-item">COBOL</div>
                        <div class="tech-item">Selenium</div>
                        <div class="tech-item">SQL</div>
                        <div class="tech-item">DB2</div>
                        <div class="tech-item">Oracle</div>
                        <div class="tech-item">Jira</div>
                        <div class="tech-item">Jenkins</div>
                        <div class="tech-item">MongoDB</div>
                        <div class="tech-item">Postman</div>
                        <div class="tech-item">SonarCloud</div>
                    </div>
                </div>

                <div class="section">
                    <h3 class="section-title">Educación</h3>
                    <div class="education-item">
                        <strong>Especialización en IA</strong><br>
                        <small>USIL (2024-2025)</small>
                    </div>
                    <div class="education-item">
                        <strong>Bachiller en Ingeniería</strong><br>
                        <small>UPCI (2007-2012)</small>
                    </div>
                    <div class="education-item">
                        <strong>Administrador de Redes</strong><br>
                        <small>TECSUP (2012)</small>
                    </div>
                </div>

                <div class="section">
                    <h3 class="section-title">Certificaciones</h3>
                    <div class="cert-item">GAIPC™ - Generative AI Professional</div>
                    <div class="cert-item">CPEFPC™ - Prompt Engineering</div>
                    <div class="cert-item">ISTQB CTFL 4.0</div>
                    <div class="cert-item">Scrum Master SMPC®</div>
                    <div class="cert-item">AWS IA Generativa</div>
                </div>
            </aside>

            <main class="content">
                <div class="stats">
                    <div class="stat-card">
                        <div class="stat-number">9+</div>
                        <div class="stat-label">Años Experiencia</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">30%</div>
                        <div class="stat-label">Mejora en Eficiencia</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">2</div>
                        <div class="stat-label">Emprendimientos</div>
                    </div>
                </div>

                <div class="highlight">
                    <h4>🚀 Especialidades Clave & Nuevos Proyectos 2025</h4>
                    <p><strong>IA Generativa:</strong> Desarrollo de soluciones para detección de anomalías y automatización</p>
                    <p><strong>Liderazgo Ágil:</strong> Coordinación de equipos multidisciplinarios</p>
                    <p><strong>Emprendimiento en Desarrollo:</strong> Nuevos talentos QA y democratización del conocimiento</p>
                </div>

                <div class="section">
                    <h2 class="section-title">🌟 Nuevas Iniciativas 2025</h2>
                    
                    <div class="experience-item project-section">
                        <div class="job-header">
                            <div>
                                <div class="job-title">🏢 AI Testing Training & Services</div>
                                <div class="company" style="color: #16a085;">Fundadora & Consultora Principal</div>
                            </div>
                            <div class="duration">Ene 2025 - Presente</div>
                        </div>
                        
                        <div style="background: white; padding: 10px; border-radius: 6px; margin: 10px 0; text-align: center; border-left: 3px solid #16a085;">
                            <em style="color: #2c3e50; font-size: 14px;">"Transformamos profesionales IT en Quality Engineers certificados internacionalmente"</em>
                        </div>
                        
                        <div class="services-grid">
                            <div class="service-card">
                                <h5>📚 CAPACITACIÓN & CERTIFICACIÓN</h5>
                                <ul>
                                    <li>✅ Fundamentos del Analista de Calidad</li>
                                    <li>✅ Capacitación basada en ISTQB</li>
                                    <li>✅ Testing Manual y Automatizado</li>
                                    <li>✅ Mentoría personalizada</li>
                                </ul>
                            </div>
                            <div class="service-card">
                                <h5>⚙️ SERVICIOS DE CALIDAD</h5>
                                <ul>
                                    <li>✅ Testing web y móvil</li>
                                    <li>✅ Automatización de pruebas</li>
                                    <li>✅ Auditorías de calidad</li>
                                    <li>✅ Testing de APIs</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <div class="experience-item podcast-section">
                        <div class="job-header">
                            <div>
                                <div class="job-title">🎙️ Podcast QA-blando</div>
                                <div class="company" style="color: #e91e63;">Host & Creadora de Contenido</div>
                            </div>
                            <div class="duration">Ene 2025 - Presente</div>
                        </div>
                        
                        <div class="philosophy-box">
                            <h4>"Serios pero no tan serios"</h4>
                            <p style="margin: 0; font-size: 12px;">Democratizando el conocimiento en calidad de software para la comunidad hispanohablante</p>
                        </div>
                        
                        <div class="services-grid">
                            <div class="service-card" style="border-left-color: #e91e63;">
                                <h5>🎤 Contenido Educativo</h5>
                                <ul>
                                    <li>📻 Tips prácticos de QA</li>
                                    <li>📻 Entrevistas a expertos</li>
                                    <li>📻 Casos de estudio reales</li>
                                    <li>📻 Tendencias en testing</li>
                                </ul>
                            </div>
                            <div class="service-card" style="border-left-color: #ffc107;">
                                <h5>🌟 Impacto Social</h5>
                                <ul>
                                    <li>🌍 Acceso gratuito al conocimiento</li>
                                    <li>🌍 Comunidad QA en español</li>
                                    <li>🌍 Mentoría a nuevos talentos</li>
                                    <li>🌍 Networking profesional</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="section">
                    <h2 class="section-title">Competencias Principales</h2>
                    
                    <div class="skill-category">
                        <h4>🔍 Aseguramiento y Control de Calidad</h4>
                        <div class="skill-item">Análisis y estrategias de prueba personalizadas</div>
                        <div class="skill-item">Supervisión de ciclos completos de testing</div>
                        <div class="skill-item">Optimización de procesos y reducción de tiempos</div>
                        <div class="skill-item">Evaluación CMMI3 y estándares de calidad</div>
                    </div>

                    <div class="skill-category">
                        <h4>🤖 IA Generativa & Automatización</h4>
                        <div class="skill-item">Soluciones basadas en IA para detección de anomalías</div>
                        <div class="skill-item">Automatización de pruebas con técnicas de IA</div>
                        <div class="skill-item">Desarrollo en Python, Java, COBOL y Selenium</div>
                        <div class="skill-item">Gestión de BD: SQL, DB2, Oracle</div>
                    </div>

                    <div class="skill-category">
                        <h4>👥 Liderazgo & Gestión</h4>
                        <div class="skill-item">Coordinación de equipos multidisciplinarios</div>
                        <div class="skill-item">Capacitación en metodologías ágiles</div>
                        <div class="skill-item">Gestión de recursos y presupuestos</div>
                        <div class="skill-item">Herramientas: Jira, Xray, Jenkins, Bitbucket</div>
                    </div>
                </div>

                <div class="section">
                    <h2 class="section-title">Experiencia Profesional Destacada</h2>

                    <div class="experience-item">
                        <div class="job-header">
                            <div>
                                <div class="job-title">Analista Senior de Aseguramiento y Control de Calidad</div>
                                <div class="company">La Positiva Seguros</div>
                            </div>
                            <div class="duration">Oct 2022 - Presente</div>
                        </div>
                        <ul class="achievements">
                            <li><strong>Liderazgo:</strong> Coordinación de equipos de calidad y supervisión de Automatización</li>
                            <li><strong>Optimización:</strong> Reducción del 20% en costos operativos</li>
                            <li><strong>IA Implementada:</strong> Aumento del 30% en velocidad de pruebas</li>
                            <li><strong>Capacitación:</strong> Desarrollo profesional en IA, Jenkins y Selenium</li>
                        </ul>
                    </div>

                    <div class="experience-item">
                        <div class="job-header">
                            <div>
                                <div class="job-title">Analista Funcional QA Senior</div>
                                <div class="company">Indra - Proyecto BBVA</div>
                            </div>
                            <div class="duration">Jul 2021 - Sep 2022</div>
                        </div>
                        <ul class="achievements">
                            <li><strong>Core Transactional:</strong> Aseguramiento en transferencias interbancarias</li>
                            <li><strong>Optimización:</strong> Reducción del 15% en tiempo de ejecución</li>
                            <li><strong>Proyectos Clave:</strong> Participación en Vocalink y liderazgo en Proyecto CIRCULAR</li>
                        </ul>
                    </div>

                    <div class="experience-item">
                        <div class="job-header">
                            <div>
                                <div class="job-title">Analista Técnico Senior</div>
                                <div class="company">Canvia - Proyectos NIUVIZ, CLARO, BBVA</div>
                            </div>
                            <div class="duration">Oct 2018 - May 2021</div>
                        </div>
                        <ul class="achievements">
                            <li><strong>VISANET:</strong> Liderazgo en pruebas de omnicanalidad, innovación y CRM</li>
                            <li><strong>Reducción de Incidentes:</strong> 20% menos incidentes en producción</li>
                            <li><strong>Múltiples Proyectos:</strong> CLARO, BBVA con mejoras significativas</li>
                        </ul>
                    </div>

                    <div class="experience-item">
                        <div class="job-header">
                            <div>
                                <div class="job-title">Roles Previos - Analista Funcional & Developer</div>
                                <div class="company">MDP Consulting, Globokas, Everis, TCS</div>
                            </div>
                            <div class="duration">2014 - 2018</div>
                        </div>
                        <ul class="achievements">
                            <li><strong>Sectores:</strong> Bancario, Telecomunicaciones, Medios de Pago</li>
                            <li><strong>Especialización:</strong> COBOL, SOA, Integración de Servicios</li>
                            <li><strong>Metodologías:</strong> Ágil, Cascada, PAR</li>
                            <li><strong>Estándares:</strong> CMMI3 y CMMI5, mejora continua</li>
                        </ul>
                    </div>
                </div>
                
                <div class="contact-footer">
                    <strong>📋 PROYECTOS Y CAPACITACIONES</strong><br>
                    📧 E-mail: aitestingservicesperu@gmail.com<br>
                    📞 Teléfono: +51 992 097 896
                </div>
            </main>
        </div>
    </div>

    <button class="download-btn" onclick="window.print()">
        📄 Descargar PDF
    </button>

    <script>
        // Optimización para impresión
        window.addEventListener('beforeprint', function() {
            document.body.style.fontSize = '11px';
        });

        window.addEventListener('afterprint', function() {
            document.body.style.fontSize = '14px';
        });

        // Función para generar PDF
        function generatePDF() {
            // Ajustar estilos para PDF
            const originalStyle = document.body.style.cssText;
            document.body.style.cssText += 'font-size: 11px !important;';
            
            // Imprimir
            window.print();
            
            // Restaurar estilos
            setTimeout(() => {
                document.body.style.cssText = originalStyle;
            }, 1000);
        }

        // Optimizar botón
        document.querySelector('.download-btn').onclick = generatePDF;
    </script>
</body>
</html>
