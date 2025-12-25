<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Liquorfistel Lösungswege & Spezialisten</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: linear-gradient(135deg, #e0f2fe 0%, #ddd6fe 100%);
            padding: 20px;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .header {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin-bottom: 30px;
            display: flex;
            gap: 20px;
            align-items: start;
        }
        
        .alert-icon {
            width: 40px;
            height: 40px;
            background: #ef4444;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 24px;
            flex-shrink: 0;
        }
        
        h1 {
            color: #1f2937;
            font-size: 28px;
            margin-bottom: 10px;
        }
        
        .subtitle {
            color: #6b7280;
            font-size: 16px;
        }
        
        .nav-tabs {
            background: white;
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin-bottom: 30px;
            overflow: hidden;
            display: flex;
            flex-wrap: wrap;
        }
        
        .nav-tab {
            flex: 1;
            min-width: 150px;
            padding: 20px;
            background: white;
            border: none;
            cursor: pointer;
            font-size: 16px;
            font-weight: 500;
            color: #6b7280;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        
        .nav-tab:hover {
            background: #f9fafb;
        }
        
        .nav-tab.active {
            background: #4f46e5;
            color: white;
        }
        
        .tab-content {
            display: none;
        }
        
        .tab-content.active {
            display: block;
        }
        
        .card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
        
        .info-box {
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
            border-left: 4px solid;
        }
        
        .info-box.warning {
            background: #fef3c7;
            border-color: #f59e0b;
            color: #92400e;
        }
        
        .info-box.danger {
            background: #fee2e2;
            border-color: #ef4444;
            color: #991b1b;
        }
        
        .info-box.info {
            background: #dbeafe;
            border-color: #3b82f6;
            color: #1e40af;
        }
        
        .info-box.success {
            background: #d1fae5;
            border-color: #10b981;
            color: #065f46;
        }
        
        .info-box h3 {
            font-size: 18px;
            margin-bottom: 10px;
            font-weight: 600;
        }
        
        .info-box ul {
            margin-left: 20px;
            margin-top: 10px;
        }
        
        .info-box li {
            margin: 5px 0;
            font-size: 14px;
        }
        
        .klinik-card {
            background: white;
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin-bottom: 20px;
            overflow: hidden;
        }
        
        .priority-badge {
            padding: 5px;
            text-align: center;
            color: white;
            font-size: 12px;
            font-weight: bold;
        }
        
        .priority-high {
            background: #ef4444;
        }
        
        .priority-medium {
            background: #f97316;
        }
        
        .klinik-content {
            padding: 25px;
        }
        
        .klinik-header {
            display: flex;
            justify-content: space-between;
            align-items: start;
            margin-bottom: 20px;
        }
        
        .klinik-title {
            font-size: 18px;
            font-weight: bold;
            color: #1f2937;
            margin-bottom: 5px;
        }
        
        .klinik-leiter {
            color: #4f46e5;
            font-weight: 500;
            font-size: 14px;
        }
        
        .klinik-icon {
            width: 40px;
            height: 40px;
            background: #e0e7ff;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #4f46e5;
            font-size: 24px;
        }
        
        .klinik-detail {
            display: flex;
            gap: 10px;
            margin: 10px 0;
            font-size: 14px;
            color: #4b5563;
            align-items: start;
        }
        
        .klinik-detail-icon {
            flex-shrink: 0;
            margin-top: 2px;
        }
        
        .klinik-highlight {
            background: #eef2ff;
            padding: 15px;
            border-radius: 10px;
            margin-top: 15px;
            font-size: 13px;
            color: #3730a3;
            font-weight: 500;
        }
        
        .step-card {
            background: white;
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            padding: 25px;
            margin-bottom: 20px;
        }
        
        .step-header {
            display: flex;
            gap: 15px;
            align-items: start;
            margin-bottom: 20px;
        }
        
        .step-number {
            width: 35px;
            height: 35px;
            background: #4f46e5;
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 18px;
            flex-shrink: 0;
        }
        
        .step-title {
            flex: 1;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .step-title h3 {
            font-size: 18px;
            color: #1f2937;
        }
        
        .checkbox {
            width: 30px;
            height: 30px;
            border: 2px solid #d1d5db;
            border-radius: 8px;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s;
        }
        
        .checkbox:hover {
            background: #f3f4f6;
        }
        
        .checkbox.checked {
            background: #dcfce7;
            border-color: #10b981;
            color: #10b981;
        }
        
        .step-details {
            margin-left: 50px;
        }
        
        .step-details ul {
            list-style: none;
        }
        
        .step-details li {
            display: flex;
            gap: 10px;
            margin: 10px 0;
            font-size: 14px;
            color: #4b5563;
        }
        
        .arrow-icon {
            color: #4f46e5;
            flex-shrink: 0;
            margin-top: 2px;
        }
        
        .timeline-card {
            background: linear-gradient(135deg, #10b981 0%, #059669 100%);
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            padding: 25px;
            color: white;
            margin-top: 20px;
        }
        
        .timeline-card h3 {
            font-size: 18px;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .timeline-card p {
            margin: 8px 0;
            font-size: 14px;
        }
        
        .question-card {
            background: #f9fafb;
            padding: 20px;
            border-radius: 10px;
            margin: 15px 0;
            transition: all 0.3s;
            display: flex;
            gap: 15px;
            align-items: start;
        }
        
        .question-card:hover {
            background: #eef2ff;
        }
        
        .question-number {
            width: 30px;
            height: 30px;
            background: #e0e7ff;
            color: #4f46e5;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 14px;
            flex-shrink: 0;
        }
        
        .question-text {
            flex: 1;
            color: #1f2937;
            font-size: 14px;
        }
        
        .footer-card {
            background: linear-gradient(135deg, #4f46e5 0%, #7c3aed 100%);
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            padding: 30px;
            color: white;
            margin-top: 30px;
        }
        
        .footer-card h3 {
            font-size: 20px;
            margin-bottom: 15px;
        }
        
        .footer-card p {
            font-size: 14px;
            line-height: 1.8;
        }
        
        @media (max-width: 768px) {
            .nav-tab {
                min-width: 120px;
                padding: 15px 10px;
                font-size: 14px;
            }
            
            h1 {
                font-size: 22px;
            }
            
            .klinik-header {
                flex-direction: column;
            }
        }
        
        @media print {
            body {
                background: white;
            }
            
            .nav-tabs {
                display: none;
            }
            
            .tab-content {
                display: block !important;
                page-break-before: always;
            }
            
            .checkbox {
                display: none;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="header">
            <div class="alert-icon">⚠</div>
            <div>
                <h1>Liquorfistel-Lösungswege</h1>
                <p class="subtitle">Rezidivierende Flüssigkeitsansammlung nach 8 OPs - Systematischer Plan für spezialisierte Hilfe</p>
            </div>
        </div>

        <!-- Navigation -->
        <div class="nav-tabs">
            <button class="nav-tab active" onclick="showTab('situation')">
                📋 Situation
            </button>
            <button class="nav-tab" onclick="showTab('kliniken')">
                🏥 Spezialkliniken
            </button>
            <button class="nav-tab" onclick="showTab('schritte')">
                ✓ Nächste Schritte
            </button>
            <button class="nav-tab" onclick="showTab('fragen')">
                💬 Wichtige Fragen
            </button>
        </div>

        <!-- Tab: Situation -->
        <div id="situation" class="tab-content active">
            <div class="card">
                <h2 style="margin-bottom: 20px; color: #1f2937; display: flex; align-items: center; gap: 10px;">
                    📋 Medizinische Einschätzung
                </h2>
                
                <div class="info-box warning">
                    <h3>Diagnose wahrscheinlich:</h3>
                    <p><strong>Rezidivierende Liquorfistel</strong> (Rhinoliquorrhoe oder spontane intrakranielle Hypotension) - Eine pathologische Verbindung zwischen Liquorraum und Außenwelt, die sich trotz 8 Operationen immer wieder bildet.</p>
                </div>

                <div class="info-box danger">
                    <h3>Kritische Situation:</h3>
                    <ul>
                        <li>8 OPs ohne dauerhaften Erfolg → akute Spezialisierung nötig</li>
                        <li>Erhöhtes Meningitis-Risiko (5-10% bei Liquorfisteln über 7 Tage)</li>
                        <li>Ursache ungeklärt → falsche OP-Technik oder übersehene Grunderkrankung?</li>
                    </ul>
                </div>

                <div class="info-box info">
                    <h3>Mögliche Ursachen bei Rezidiven:</h3>
                    <ul>
                        <li><strong>Erhöhter intrakranieller Druck</strong> (drückt Transplantat raus)</li>
                        <li><strong>Falsche Verschlusstechnik</strong> (underlay vs. onlay vs. sandwich)</li>
                        <li><strong>Übersehene zweite Fistelstelle</strong></li>
                        <li><strong>Angeborene Knochendefekte</strong> oder Dura-Schwachstellen</li>
                        <li><strong>Adipositas</strong> (bei spontanen Fisteln Risikofaktor)</li>
                    </ul>
                </div>

                <div class="info-box success">
                    <h3>Gute Nachrichten:</h3>
                    <ul>
                        <li>98% Heilungsrate bei richtiger Behandlung durch Spezialisten</li>
                        <li>Mikrochirurgischer Verschluss kann >90% Heilung erreichen</li>
                        <li>Deutschland hat mehrere Weltklasse-Zentren für diesen Fall</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Tab: Kliniken -->
        <div id="kliniken" class="tab-content">
            <div class="klinik-card">
                <div class="priority-badge priority-high">PRIORITÄT: SEHR HOCH</div>
                <div class="klinik-content">
                    <div class="klinik-header">
                        <div>
                            <div class="klinik-title">Charité Berlin - Klinik für Neurochirurgie</div>
                            <div class="klinik-leiter">Prof. Dr. Peter Vajkoczy</div>
                        </div>
                        <div class="klinik-icon">🏥</div>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">✓</span>
                        <span><strong>Expertise:</strong> Schädelbasis, rezidivierende Liquorfisteln, über 6.000 OPs/Jahr</span>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">📞</span>
                        <span>Tel: +49 30 450 560 002</span>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">✉</span>
                        <span>neurochirurgie@charite.de</span>
                    </div>
                    <div class="klinik-highlight">
                        Führende Expertise bei komplexen, therapieresistenten Fällen
                    </div>
                </div>
            </div>

            <div class="klinik-card">
                <div class="priority-badge priority-high">PRIORITÄT: SEHR HOCH</div>
                <div class="klinik-content">
                    <div class="klinik-header">
                        <div>
                            <div class="klinik-title">Universitätsklinikum Tübingen - Neurochirurgie</div>
                            <div class="klinik-leiter">Prof. Dr. Marcos Tatagiba</div>
                        </div>
                        <div class="klinik-icon">🏥</div>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">✓</span>
                        <span><strong>Expertise:</strong> Weltweite Expertise Schädelbasischirurgie, Liquorfisteln</span>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">📞</span>
                        <span>Tel: +49 7071 29-80442</span>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">✉</span>
                        <span>neurochirurgie@med.uni-tuebingen.de</span>
                    </div>
                    <div class="klinik-highlight">
                        Renommiertes Zentrum für Schädelbasis-Operationen
                    </div>
                </div>
            </div>

            <div class="klinik-card">
                <div class="priority-badge priority-medium">PRIORITÄT: HOCH</div>
                <div class="klinik-content">
                    <div class="klinik-header">
                        <div>
                            <div class="klinik-title">Universitätsklinikum Freiburg - HNO & Neurochirurgie</div>
                            <div class="klinik-leiter">Interdisziplinäres Schädelbasiszentrum</div>
                        </div>
                        <div class="klinik-icon">🏥</div>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">✓</span>
                        <span><strong>Expertise:</strong> Endoskopische Duraplastiken, Liquorfistelverschluss</span>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">📞</span>
                        <span>Tel: +49 761 270-0</span>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">✉</span>
                        <span>info@uniklinik-freiburg.de</span>
                    </div>
                    <div class="klinik-highlight">
                        Top 5 Klinikum Deutschland, interdisziplinäres Team
                    </div>
                </div>
            </div>

            <div class="klinik-card">
                <div class="priority-badge priority-medium">PRIORITÄT: HOCH</div>
                <div class="klinik-content">
                    <div class="klinik-header">
                        <div>
                            <div class="klinik-title">Universitätsklinikum Heidelberg - Neurochirurgie</div>
                            <div class="klinik-leiter">Schädelbasischirurgie-Team</div>
                        </div>
                        <div class="klinik-icon">🏥</div>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">✓</span>
                        <span><strong>Expertise:</strong> Neuroonkologie, Schädelbasischirurgie, komplexe Fälle</span>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">📞</span>
                        <span>Tel: +49 6221 56-0</span>
                    </div>
                    <div class="klinik-detail">
                        <span class="klinik-detail-icon">✉</span>
                        <span>info@med.uni-heidelberg.de</span>
                    </div>
                    <div class="klinik-highlight">
                        Exzellente Forschung und Behandlung
                    </div>
                </div>
            </div>
        </div>

        <!-- Tab: Schritte -->
        <div id="schritte" class="tab-content">
            <div class="step-card">
                <div class="step-header">
                    <div class="step-number">1</div>
                    <div class="step-title">
                        <h3>Medizinische Unterlagen zusammenstellen</h3>
                        <div class="checkbox" onclick="toggleCheck(this)"></div>
                    </div>
                </div>
                <div class="step-details">
                    <ul>
                        <li><span class="arrow-icon">→</span> Alle CT/MRT-Bilder auf CD brennen lassen</li>
                        <li><span class="arrow-icon">→</span> Operationsberichte aller 8 OPs sammeln</li>
                        <li><span class="arrow-icon">→</span> Arztbriefe und Befunde chronologisch ordnen</li>
                        <li><span class="arrow-icon">→</span> Aktuelle Symptome dokumentieren (wann tritt Flüssigkeit auf, Menge, Begleiterscheinungen)</li>
                    </ul>
                </div>
            </div>

            <div class="step-card">
                <div class="step-header">
                    <div class="step-number">2</div>
                    <div class="step-title">
                        <h3>Zweitmeinung bei Spezialklinik einholen</h3>
                        <div class="checkbox" onclick="toggleCheck(this)"></div>
                    </div>
                </div>
                <div class="step-details">
                    <ul>
                        <li><span class="arrow-icon">→</span> Charité Berlin als erste Wahl kontaktieren (Prof. Vajkoczy)</li>
                        <li><span class="arrow-icon">→</span> Alternativ: Tübingen (Prof. Tatagiba) - ebenfalls Top-Expertise</li>
                        <li><span class="arrow-icon">→</span> Per Telefon/Email Termin für Zweitmeinungssprechstunde anfragen</li>
                        <li><span class="arrow-icon">→</span> Unterlagen vorher per Post/Upload schicken</li>
                    </ul>
                </div>
            </div>

            <div class="step-card">
                <div class="step-header">
                    <div class="step-number">3</div>
                    <div class="step-title">
                        <h3>Diagnostik klären</h3>
                        <div class="checkbox" onclick="toggleCheck(this)"></div>
                    </div>
                </div>
                <div class="step-details">
                    <ul>
                        <li><span class="arrow-icon">→</span> Fragen: Wurde Beta-2-Transferrin-Test gemacht? (beweist Liquor)</li>
                        <li><span class="arrow-icon">→</span> Wurde Fluorescein-Test durchgeführt? (zeigt genaue Leckstelle)</li>
                        <li><span class="arrow-icon">→</span> Wurde intrakranieller Druck gemessen?</li>
                        <li><span class="arrow-icon">→</span> MR-Myelographie zur Fistel-Lokalisation durchgeführt?</li>
                    </ul>
                </div>
            </div>

            <div class="step-card">
                <div class="step-header">
                    <div class="step-number">4</div>
                    <div class="step-title">
                        <h3>Ursachenforschung intensivieren</h3>
                        <div class="checkbox" onclick="toggleCheck(this)"></div>
                    </div>
                </div>
                <div class="step-details">
                    <ul>
                        <li><span class="arrow-icon">→</span> Erhöhter Hirndruck als Ursache? (kann Rezidive verursachen)</li>
                        <li><span class="arrow-icon">→</span> Adipositas als Risikofaktor? (bei spontanen Fisteln häufig)</li>
                        <li><span class="arrow-icon">→</span> Angeborene Knochendefekte möglich?</li>
                        <li><span class="arrow-icon">→</span> Wurde auf alle 3 Fisteltypen untersucht? (ventral, Divertikel, epidurale Venen)</li>
                    </ul>
                </div>
            </div>

            <div class="step-card">
                <div class="step-header">
                    <div class="step-number">5</div>
                    <div class="step-title">
                        <h3>Therapieoptionen besprechen</h3>
                        <div class="checkbox" onclick="toggleCheck(this)"></div>
                    </div>
                </div>
                <div class="step-details">
                    <ul>
                        <li><span class="arrow-icon">→</span> Warum schlägt aktuelle OP-Technik nicht an?</li>
                        <li><span class="arrow-icon">→</span> Alternative Verschlusstechniken prüfen (Sandwich, Onlay, Underlay)</li>
                        <li><span class="arrow-icon">→</span> Lumbaldrainage nach OP zur Druckentlastung?</li>
                        <li><span class="arrow-icon">→</span> Gestielter nasoseptaler Lappen als stabilere Abdeckung?</li>
                    </ul>
                </div>
            </div>

            <div class="timeline-card">
                <h3>📅 Zeitplan</h3>
                <p><strong>Diese Woche:</strong> Unterlagen zusammenstellen, Charité/Tübingen kontaktieren</p>
                <p><strong>Nächste 1-2 Wochen:</strong> Zweitmeinungstermin vereinbaren</p>
                <p><strong>Innerhalb 4 Wochen:</strong> Bei Spezialklinik vorstellen und neue Behandlungsstrategie festlegen</p>
            </div>
        </div>

        <!-- Tab: Fragen -->
        <div id="fragen" class="tab-content">
            <div class="card">
                <h2 style="margin-bottom: 10px; color: #1f2937; display: flex; align-items: center; gap: 10px;">
                    💬 Wichtige Fragen für Ärztegespräche
                </h2>
                
                <p style="color: #6b7280; margin-bottom: 25px; font-size: 14px;">
                    Diese Fragen helfen, die bisherige Behandlung zu verstehen und neue Ansätze zu finden:
                </p>
                
                <div class="question-card">
                    <div class="question-number">1</div>
                    <div class="question-text">Welche genaue OP-Technik wurde bei den 8 Eingriffen verwendet?</div>
                </div>

                <div class="question-card">
                    <div class="question-number">2</div>
                    <div class="question-text">Wurde der intrakranielle Druck gemessen und behandelt?</div>
                </div>

                <div class="question-card">
                    <div class="question-number">3</div>
                    <div class="question-text">Gibt es Hinweise auf erhöhten Hirndruck (Kopfschmerzen, Übelkeit)?</div>
                </div>

                <div class="question-card">
                    <div class="question-number">4</div>
                    <div class="question-text">Wurde die exakte Lokalisation der Fistel mit Fluorescein bestimmt?</div>
                </div>

                <div class="question-card">
                    <div class="question-number">5</div>
                    <div class="question-text">Wie schnell tritt die Flüssigkeit nach den OPs wieder auf?</div>
                </div>

                <div class="question-card">
                    <div class="question-number">6</div>
                    <div class="question-text">Gibt es Anzeichen einer Meningitis (Fieber, Nackensteifigkeit)?</div>
                </div>
