<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2do Congreso Venezolano de Constelaciones Cuánticas</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Arial', sans-serif; line-height: 1.6; color: #333; background: #faf8f2; }
        .container { max-width: 1200px; margin: 0 auto; padding: 0 20px; }
        
        .hero {
            background: linear-gradient(135deg, #D4AF37 0%, #FFD700 50%, #D4AF37 100%);
            color: #1a237e; padding: 100px 0; text-align: center;
        }
        .hero h1 { font-size: 3rem; margin-bottom: 20px; color: #1a237e; }
        .hero h2 { font-size: 1.8rem; margin-bottom: 15px; }
        
        .cta-button {
            display: inline-block; background: #1a237e; color: #FFD700;
            padding: 15px 30px; font-size: 1.2rem; text-decoration: none;
            border-radius: 50px; margin: 10px; border: 2px solid #1a237e;
            transition: all 0.3s ease;
        }
        .cta-button:hover { background: #FFD700; color: #1a237e; transform: translateY(-3px); }
        
        .section { padding: 80px 0; }
        .section-title { 
            text-align: center; font-size: 2.5rem; margin-bottom: 50px; 
            color: #1a237e; 
        }
        .section-title:after {
            content: ''; display: block; width: 100px; height: 3px;
            background: #D4AF37; margin: 15px auto;
        }
        
        .modalidad-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 30px; margin-top: 40px; }
        .modalidad-card {
            background: white; padding: 40px; border-radius: 15px;
            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.2); text-align: center;
            border-top: 5px solid #D4AF37;
        }
        
        .ponentes-grid {
            display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px; margin-top: 40px;
        }
        .ponente-card {
            background: white; border-radius: 15px; overflow: hidden;
            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.2);
            transition: transform 0.3s ease;
        }
        .ponente-card:hover { transform: translateY(-10px); }
        .ponente-img { 
            width: 100%; height: 300px; object-fit: cover;
            border-bottom: 3px solid #D4AF37;
            background: linear-gradient(45deg, #f0f0f0, #e0e0e0);
            display: flex; align-items: center; justify-content: center;
            color: #666; font-size: 1rem; text-align: center;
            padding: 20px;
        }
        .ponente-info { padding: 20px; }
        .ponente-info h4 { color: #1a237e; margin-bottom: 10px; }
        .ponente-tema { color: #D4AF37; font-weight: 600; margin-bottom: 10px; font-style: italic; }
        
        .agenda-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 30px; margin-top: 40px; }
        .agenda-dia { background: white; padding: 30px; border-radius: 15px; box-shadow: 0 10px 30px rgba(212, 175, 55, 0.2); }
        .horario-item { display: flex; margin-bottom: 15px; padding-bottom: 15px; border-bottom: 1px solid #f0f0f0; }
        .horario-hora { font-weight: 700; color: #D4AF37; min-width: 80px; }
        
        .precios-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px; margin-top: 40px; }
        .precio-card { background: white; padding: 40px 20px; border-radius: 15px; box-shadow: 0 10px 30px rgba(212, 175, 55, 0.2); text-align: center; }
        .precio-card.destacado { border: 3px solid #D4AF37; transform: scale(1.05); }
        .precio-monto { font-size: 2.5rem; font-weight: 700; color: #D4AF37; margin-bottom: 20px; }
        .precio-titulo { color: #1a237e; font-size: 1.3rem; margin-bottom: 15px; }
        .precio-desc { 
            color: #666; margin-bottom: 20px; font-size: 0.9rem; 
            background: #fff9e6; padding: 8px 15px; border-radius: 20px; 
            display: inline-block; 
        }
        
        .contacto-info { text-align: center; background: white; padding: 40px; border-radius: 15px; box-shadow: 0 10px 30px rgba(212, 175, 55, 0.2); margin-top: 40px; }
        .contacto-buttons { display: flex; justify-content: center; gap: 20px; margin-top: 30px; flex-wrap: wrap; }
        
        @media (max-width: 768px) {
            .modalidad-grid, .agenda-grid { grid-template-columns: 1fr; }
            .hero h1 { font-size: 2rem; }
            .contacto-buttons { flex-direction: column; align-items: center; }
            .precio-card.destacado { transform: none; }
        }
    </style>
</head>
<body>
    <!-- HERO SECTION -->
    <section class="hero">
        <div class="container">
            <h1>2do Congreso Venezolano de Constelaciones Cuánticas</h1>
            <h2>Modalidad Híbrida: Presencial 15 Nov + Online 16 Nov</h2>
            <h3>Exclusivo para Terapeutas y Personas en Formación</h3>
            <a href="#inscripcion" class="cta-button">🎫 Reservar Mi Cupo - Desde $20</a>
            <a href="#agenda" class="cta-button">📅 Ver Agenda Completa</a>
        </div>
    </section>

    <!-- MODALIDAD SECTION -->
    <section class="section">
        <div class="container">
            <h2 class="section-title">Vive la Experiencia Completa</h2>
            <div class="modalidad-grid">
                <div class="modalidad-card">
                    <h3>📍 Sábado 15 Nov - Presencial</h3>
                    <p><strong>OVA Ccs. Centro Comercial Plaza La Boyera, Nivel A, local OVA. Vía el Hatillo. Caracas</strong></p>
                    <p>Capacidad limitada: 30 personas</p>
                    <ul>
                        <li>6 facilitadoras expertas en vivo</li>
                        <li>Constelaciones presenciales</li>
                        <li>Networking directo</li>
                        <li>Material físico exclusivo</li>
                        <li>Horario: 9:00 AM - 3:00 PM</li>
                    </ul>
                </div>
                <div class="modalidad-card">
                    <h3>🌐 Domingo 16 Nov - Online</h3>
                    <p><strong>Transmisión en vivo desde cualquier lugar</strong></p>
                    <p>Acceso internacional</p>
                    <ul>
                        <li>8 expertos internacionales y nacionales</li>
                        <li>Sesión especial con Clara Prchal</li>
                        <li>Grabaciones por 30 días</li>
                        <li>Certificado digital</li>
                        <li>Horario: 9:00 AM - 4:00 PM</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- PONENTES PRESENCIALES -->
    <section class="section" style="background: #f0f2ff;">
        <div class="container">
            <h2 class="section-title">Ponentes Presenciales - Sábado 15 Nov</h2>
            <div class="ponentes-grid">
                <div class="ponente-card">
                    <div class="ponente-img">
                        Yusmerly Medina Chávez<br>
                        <em>"Fundamentos de la Conexión Cuántica"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Yusmerly Medina Chávez</h4>
                        <div class="ponente-tema">"Fundamentos de la Conexión Cuántica en Sistemas Familiares"</div>
                        <div class="ponente-bio">Psicóloga, Consteladora Familiar. Hipnoterapeuta. Coach de Bienestar. Especialista en Análisis Transaccional. Formadora en Constelación Familiar Transaccional. Fundadora de Cross Focus Integral.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Natali Moreno<br>
                        <em>"Orden Invisible de los Negocios Conscientes"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Natali Moreno</h4>
                        <div class="ponente-tema">"Orden Invisible de los Negocios Conscientes"</div>
                        <div class="ponente-bio">Mentora Sistémica | Consteladora Familiar y de Negocios. Guío espacios de transformación para quienes están listos para verse, reconocerse y liberarse.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Mariella Urbano<br>
                        <em>"Integrando la Hipnosis Profunda"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Mariella Urbano</h4>
                        <div class="ponente-tema">"Integrando la Hipnosis Profunda en las Dinámicas de las Constelaciones"</div>
                        <div class="ponente-bio">Doctora en Educación, Magíster en Administración, Psicoterapeuta Gestáltica y Especialista en Dinámicas de Grupo. Maestra en procesos de transformación emocional, espiritual y sistémica.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Teresa Egaña<br>
                        <em>"Constelaciones y Arquetipos Femeninos"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Teresa Egaña</h4>
                        <div class="ponente-tema">"Cuando las Constelaciones Danzan Entre Arquetipos y La Mujer"</div>
                        <div class="ponente-bio">Speaker & Viajera Transformacional. Investigadora de La Otra Historia De La Mujer & Del Arquetipo De La Magdalena. Multi-Galardonada internacionalmente. Consteladora Sistémica. Fundadora de MUJER WOW</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Laura Acevedo<br>
                        <em>"Reactivación del Ser - Modelo 4R"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Laura Acevedo</h4>
                        <div class="ponente-tema">"Constelaciones Cuánticas para la Reactivación del Ser, modelo de las 4R"</div>
                        <div class="ponente-bio">Comunicadora Social, educadora y psicoterapeuta transpersonal. Autora del método de Constelaciones Cuánticas para la reactivación del ser y las 4R. Conferencista internacional, directora de la Escuela Revela Tu Ser.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Aracelys Hernández<br>
                        <em>"Activación del ADN"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Aracelys Hernández</h4>
                        <div class="ponente-tema">"Activación del ADN"</div>
                        <div class="ponente-bio">Médico Pediatra especializada en sanación integral, Consteladora Familiar, Medicina Tradicional China, Máster PNL, TRE, Activación del ADN y Bio Desprogramación Emocional</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- PONENTES ONLINE -->
    <section class="section">
        <div class="container">
            <h2 class="section-title">Ponentes Online - Domingo 16 Nov</h2>
            <div class="ponentes-grid">
                <div class="ponente-card">
                    <div class="ponente-img">
                        Clara Prchal<br>
                        <em>"Hipnoterapia Expansiva"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Clara Prchal (Invitada Especial)</h4>
                        <div class="ponente-tema">"Hipnoterapia Expansiva y Movimiento Sistémico"</div>
                        <div class="ponente-bio">Psicóloga, Hipnoterapeuta, Terapeuta Sistémica, instructora de Mindfulness y de Movimiento Expresivo. Fundadora de la Certificación Internacional HEART.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Astrid Kessert<br>
                        <em>"Conexiones Sagradas"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Astrid Kessert</h4>
                        <div class="ponente-tema">"Conexiones Sagradas: De Lo Terrenal a Lo Intangible"</div>
                        <div class="ponente-bio">Directora y Fundadora Constelaciones familiares y Organizacionales, Terapia de Contención, Pedagogía Sistémica. Trauma social.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Kelssy Chacón Pinto<br>
                        <em>"Recalibración Sistémica"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Kelssy Chacón Pinto</h4>
                        <div class="ponente-tema">"Manual de Recalibración Sistémica"</div>
                        <div class="ponente-bio">Formadora en Constelaciones Cuánticas en Kelssy Academy-Miami. Terapeuta Energética y Holística. Experta en Dispositivo Cuántico HEALY, aprobado por la FDA en EEUU.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Cecilia Rodríguez<br>
                        <em>"Liderazgo Femenino"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Cecilia Rodríguez</h4>
                        <div class="ponente-tema">"De la Lealtad Invisible al Liderazgo Femenino: Un viaje sistémico de la mujer consciente"</div>
                        <div class="ponente-bio">Consteladora y Coach Sistémica, Mentora en liderazgo femenino y reconexión con la fuerza ancestral.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Italia y Sonia Campora<br>
                        <em>"Tarot Cuántico"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Italia y Sonia Campora</h4>
                        <div class="ponente-tema">"El Tarot Cuántico"</div>
                        <div class="ponente-bio">Son magísteres en Educación, especialistas en psicoterapia y terapias holísticas. Coautoras del Tarot Cuántico, Mindful Trail y la Bioreprogramación Holística. Dirigen el Centro Holístico Holoss.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Fernando Fermín<br>
                        <em>"Ordenamiento de Consciencia"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Fernando Fermín</h4>
                        <div class="ponente-tema">"Ordenamiento de Consciencia Humana"</div>
                        <div class="ponente-bio">Artista del espíritu. Ordenamientos de consciencia humana.</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Albis Rivas Rivas<br>
                        <em>"Preguntas Benevolentes"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Albis Rivas Rivas</h4>
                        <div class="ponente-tema">"Las Preguntas Benevolentes y El Campo Cuántico"</div>
                        <div class="ponente-bio">Docente en Lengua y Literatura. Magister en ciencias mención Orientación para Padres. Consteladora Familiar. Directora del Centro de Estudios y Crecimiento en Familia</div>
                    </div>
                </div>
                <div class="ponente-card">
                    <div class="ponente-img">
                        Karina Merlo y Milagros Ortega<br>
                        <em>"Melodías Ancestrales"</em>
                    </div>
                    <div class="ponente-info">
                        <h4>Karina Merlo y Milagros Ortega</h4>
                        <div class="ponente-tema">"Las Melodías Viajan En Mí A Través De Mis Ancestros"</div>
                        <div class="ponente-bio">Especialistas en constelaciones familiares y fluviales, creadoras de la formación Melodías Sistémicas del Corazón y líderes de la escuela Ecosic.</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- AGENDA SECTION -->
    <section id="agenda" class="section" style="background: #f0f2ff;">
        <div class="container">
            <h2 class="section-title">Agenda Detallada</h2>
            <div class="agenda-grid">
                <div class="agenda-dia">
                    <h3>📍 Sábado 15 - Presencial</h3>
                    <div class="horario-item"><div class="horario-hora">9:00 AM</div><div class="horario-actividad">Registro y Apertura</div></div>
                    <div class="horario-item"><div class="horario-hora">9:40 AM</div><div class="horario-actividad">Yusmerly Medina - Apertura</div></div>
                    <div class="horario-item"><div class="horario-hora">10:20 AM</div><div class="horario-actividad">Natali Moreno - Orden Invisible de los Negocios Conscientes</div></div>
                    <div class="horario-item"><div class="horario-hora">10:50 AM</div><div class="horario-actividad">Receso</div></div>
                    <div class="horario-item"><div class="horario-hora">11:10 AM</div><div class="horario-actividad">Mariella Urbano - Integrando la Hipnosis Profunda</div></div>
                    <div class="horario-item"><div class="horario-hora">12:00 PM</div><div class="horario-actividad">Almuerzo</div></div>
                    <div class="horario-item"><div class="horario-hora">1:00 PM</div><div class="horario-actividad">Teresa Egaña - Constelaciones y Arquetipos Femeninos</div></div>
                    <div class="horario-item"><div class="horario-hora">1:40 PM</div><div class="horario-actividad">Laura Acevedo - Reactivación del Ser con 4R</div></div>
                    <div class="horario-item"><div class="horario-hora">2:20 PM</div><div class="horario-actividad">Aracelys Hernández - Activación del ADN</div></div>
                    <div class="horario-item"><div class="horario-hora">3:00 PM</div><div class="horario-actividad">Cierre</div></div>
                </div>
                <div class="agenda-dia">
                    <h3>🌐 Domingo 16 - Online</h3>
                    <div class="horario-item"><div class="horario-hora">9:00 AM</div><div class="horario-actividad">Yusmerly Medina - Apertura Virtual</div></div>
                    <div class="horario-item"><div class="horario-hora">9:10 AM</div><div class="horario-actividad">Clara Prchal - Hipnoterapia Expansiva</div></div>
                    <div class="horario-item"><div class="horario-hora">9:40 AM</div><div class="horario-actividad">Albis Rivas - Preguntas Benevolentes</div></div>
                    <div class="horario-item"><div class="horario-hora">10:10 AM</div><div class="horario-actividad">Receso</div></div>
                    <div class="horario-item"><div class="horario-hora">10:20 AM</div><div class="horario-actividad">Fernando Fermín - Ordenamiento de Consciencia</div></div>
                    <div class="horario-item"><div class="horario-hora">10:50 AM</div><div class="horario-actividad">Italia y Sonia Campora - Tarot Cuántico</div></div>
                    <div class="horario-item"><div class="horario-hora">11:20 AM</div><div class="horario-actividad">Cecilia Rodríguez - Liderazgo Femenino</div></div>
                    <div class="horario-item"><div class="horario-hora">12:00 PM</div><div class="horario-actividad">Almuerzo</div></div>
                    <div class="horario-item"><div class="horario-hora">1:00 PM</div><div class="horario-actividad">Kelssy Chacón - Recalibración Sistémica</div></div>
                    <div class="horario-item"><div class="horario-hora">1:30 PM</div><div class="horario-actividad">Astrid Kessert - Conexiones Sagradas</div></div>
                    <div class="horario-item"><div class="horario-hora">2:00 PM</div><div class="horario-actividad">Receso</div></div>
                    <div class="horario-item"><div class="horario-hora">2:30 PM</div><div class="horario-actividad">Karina Merlo y Milagros Ortega - Melodías Ancestrales</div></div>
                    <div class="horario-item"><div class="horario-hora">3:10 PM</div><div class="horario-actividad">Sesión de preguntas</div></div>
                    <div class="horario-item"><div class="horario-hora">3:40 PM</div><div class="horario-actividad">Cierre</div></div>
                </div>
            </div>
        </div>
    </section>

    <!-- PRECIOS SECTION -->
    <section id="inscripcion" class="section">
        <div class="container">
            <h2 class="section-title">Inversión Accesible</h2>
            <div class="precios-grid">
                <div class="precio-card">
                    <div class="precio-titulo">💰 Pago en Efectivo</div>
                    <div class="precio-monto">$20</div>
                    <div class="precio-desc">20% de descuento</div>
                    <p>Recepción en oficinas de Cross Focus Integral</p>
                    <a href="https://api.whatsapp.com/send?phone=584142254448&text=Hola!%20Quiero%20inscribirme%20en%20el%20congreso%20con%20pago%20en%20efectivo%20(%2420)" class="cta-button" style="font-size: 1rem;">Reservar con Efectivo</a>
                </div>
                <div class="precio-card">
                    <div class="precio-titulo">🇻🇪 Pago en Bolívares</div>
                    <div class="precio-monto">$25</div>
                    <div class="precio-desc">Equivalente en BS tasa BCV</div>
                    <p>Pago Móvil al 0414-225-4448<br>Banesco o Banco de Venezuela</p>
                    <a href="https://api.whatsapp.com/send?phone=584142254448&text=Hola!%20Quiero%20inscribirme%20en%20el%20congreso%20con%20pago%20en%20bolívares%20(%2425)" class="cta-button" style="font-size: 1rem;">Pagar en Bolívares</a>
                </div>
                <div class="precio-card destacado">
                    <div class="precio-titulo">🌍 Pago Internacional</div>
                    <div class="precio-monto">$35</div>
                    <div class="precio-desc">Para participantes fuera de Venezuela</div>
                    <p>Pago seguro por PayPal</p>
                    <!-- ENLACE PAYPAL CORREGIDO -->
                    <a href="https://www.paypal.com/paypalme/yusmerlymedina/35" class="cta-button" style="font-size: 1rem;">Pagar con PayPal</a>
                </div>
            </div>
        </div>
    </section>

    <!-- CONTACTO SECTION -->
    <section class="section" style="background: #f0f2ff;">
        <div class="container">
            <h2 class="section-title">¿Tienes Preguntas?</h2>
            <div class="contacto-info">
                <p>Estamos aquí para ayudarte. Contáctanos directamente:</p>
                <div class="contacto-buttons">
                    <a href="https://api.whatsapp.com/send?phone=584142254448&text=Hola!%20Quiero%20más%20información%20sobre%20el%20Congreso%20de%20Constelaciones%20Cuánticas" class="cta-button">📱 WhatsApp</a>
                    <a href="mailto:cvconstelacionescuanticas@gmail.com?subject=Información%20Congreso%20Constelaciones%20Cuánticas&body=Hola!%20Me%20interesa%20el%20congreso%20y%20quiero%20más%20información" class="cta-button">✉️ Email</a>
                    <a href="https://instagram.com/cvconstelacionescuanticas" class="cta-button">📸 Instagram</a>
                </div>
                <p style="margin-top: 20px;">
                    <strong>Email:</strong> cvconstelacionescuanticas@gmail.com<br>
                    <strong>Teléfono:</strong> +58 414-225-4448<br>
                    <strong>Web:</strong> www.crossfocusintegral.com
                </p>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer style="background: #1a237e; color: #FFD700; padding: 40px 0; text-align: center;">
        <div class="container">
            <p>&copy; 2024 2do Congreso Venezolano de Constelaciones Cuánticas. Todos los derechos reservados.</p>
            <p>Organizado por Yusmerly Medina | Cross Focus Integral</p>
        </div>
    </footer>
</body>
</html>
