

<html lang="pt-BR">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">

    <meta name="theme-color" content="#4CAF50">

    <meta name="apple-mobile-web-app-capable" content="yes">

    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">

    <title>Meu Planejador</title>

    

    <!-- Manifest for PWA -->

    <link rel="manifest" href="data:application/json,{&quot;name&quot;:&quot;Meu Planejador&quot;,&quot;short_name&quot;:&quot;Planejador&quot;,&quot;start_url&quot;:&quot;/&quot;,&quot;display&quot;:&quot;standalone&quot;,&quot;background_color&quot;:&quot;#ffffff&quot;,&quot;theme_color&quot;:&quot;#4CAF50&quot;,&quot;orientation&quot;:&quot;portrait&quot;,&quot;icons&quot;:[{&quot;src&quot;:&quot;data:image/png;base64,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&quot;,&quot;sizes&quot;:&quot;192x192&quot;,&quot;type&quot;:&quot;image/png&quot;}]}">

    

    <style>

        * {

            margin: 0;

            padding: 0;

            box-sizing: border-box;

            -webkit-tap-highlight-color: transparent;

        }

        

        body {

            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;

            background: #f0f2f5;

            color: #333;

            height: 100vh;

            overflow: hidden;

            user-select: none;

        }

        

        .container {

            max-width: 100%;

            height: 100vh;

            display: flex;

            flex-direction: column;

            background: white;

        }

        

        header {

            background: linear-gradient(135deg, #4CAF50, #45a049);

            color: white;

            padding: 1rem;

            box-shadow: 0 2px 10px rgba(0,0,0,0.1);

            position: relative;

            z-index: 100;

        }

        

        h1 {

            font-size: 1.5rem;

            font-weight: 600;

            text-align: center;

        }

        

        .nav-tabs {

            display: flex;

            background: white;

            box-shadow: 0 2px 5px rgba(0,0,0,0.1);

            overflow-x: auto;

            scrollbar-width: none;

            -webkit-overflow-scrolling: touch;

        }

        

        .nav-tabs::-webkit-scrollbar {

            display: none;

        }

        

        .nav-tab {

            flex: 1;

            min-width: max-content;

            padding: 0.75rem 1rem;

            border: none;

            background: none;

            cursor: pointer;

            font-size: 0.9rem;

            color: #666;

            border-bottom: 3px solid transparent;

            transition: all 0.3s ease;

            white-space: nowrap;

        }

        

        .nav-tab.active {

            color: #4CAF50;

            border-bottom-color: #4CAF50;

            font-weight: 600;

        }

        

        .nav-tab:active {

            background: #f5f5f5;

        }

        

        .content {

            flex: 1;

            overflow-y: auto;

            -webkit-overflow-scrolling: touch;

            padding: 1rem;

            padding-bottom: 80px;

        }

        

        .tab-content {

            display: none;

            animation: fadeIn 0.3s ease;

        }

        

        .tab-content.active {

            display: block;

        }

        

        @keyframes fadeIn {

            from { opacity: 0; transform: translateY(10px); }

            to { opacity: 1; transform: translateY(0); }

        }

        

        /* Full-screen event alert */

        .event-alert-overlay {

            position: fixed;

            top: 0;

            left: 0;

            width: 100%;

            height: 100%;

            background: rgba(255, 0, 0, 0.95);

            z-index: 9999;

            display: none;

            align-items: center;

            justify-content: center;

            flex-direction: column;

            animation: pulseAlert 1s ease-in-out infinite;

        }

        

        .event-alert-overlay.show {

            display: flex;

        }

        

        @keyframes pulseAlert {

            0%, 100% { background: rgba(255, 0, 0, 0.95); }

            50% { background: rgba(255, 50, 50, 0.98); }

        }

        

        .event-alert-content {

            text-align: center;

            color: white;

            padding: 2rem;

            animation: scaleIn 0.5s ease;

        }

        

        @keyframes scaleIn {

            from { transform: scale(0.5); opacity: 0; }

            to { transform: scale(1); opacity: 1; }

        }

        

        .event-alert-icon {

            font-size: 6rem;

            margin-bottom: 1rem;

            animation: bounce 1s ease-in-out infinite;

        }

        

        @keyframes bounce {

            0%, 100% { transform: translateY(0); }

            50% { transform: translateY(-20px); }

        }

        

        .event-alert-title {

            font-size: 3rem;

            font-weight: bold;

            margin-bottom: 1rem;

            text-transform: uppercase;

            letter-spacing: 2px;

        }

        

        .event-alert-event {

            font-size: 2rem;

            margin-bottom: 2rem;

            padding: 1rem;

            background: rgba(255, 255, 255, 0.2);

            border-radius: 10px;

        }

        

        .event-alert-dismiss {

            background: white;

            color: #333;

            font-size: 1.5rem;

            padding: 1rem 3rem;

            border: none;

            border-radius: 50px;

            cursor: pointer;

            font-weight: bold;

            box-shadow: 0 4px 20px rgba(0,0,0,0.3);

            transition: all 0.3s ease;

        }

        

        .event-alert-dismiss:hover {

            transform: scale(1.05);

            box-shadow: 0 6px 25px rgba(0,0,0,0.4);

        }

        

        .event-alert-dismiss:active {

            transform: scale(0.95);

        }

        

        /* Common components */

        .input-group {

            display: flex;

            gap: 0.5rem;

            margin-bottom: 1rem;

        }

        

        input[type="text"], input[type="datetime-local"], textarea {

            flex: 1;

            padding: 0.75rem;

            border: 2px solid #e0e0e0;

            border-radius: 8px;

            font-size: 1rem;

            outline: none;

            transition: border-color 0.3s ease;

        }

        

        input:focus, textarea:focus {

            border-color: #4CAF50;

        }

        

        button {

            background: #4CAF50;

            color: white;

            border: none;

            padding: 0.75rem 1.5rem;

            border-radius: 8px;

            font-size: 1rem;

            cursor: pointer;

            transition: all 0.3s ease;

            font-weight: 500;

        }

        

        button:active {

            transform: scale(0.95);

        }

        

        button:hover {

            background: #45a049;

        }



        button.gemini-btn {

            background: linear-gradient(135deg, #4285F4, #9B72F9);

        }

        button.gemini-btn:hover {

            background: linear-gradient(135deg, #3a75d8, #8a63e0);

        }

        

        .btn-secondary {

            background: #6c757d;

        }

        

        .btn-secondary:hover {

            background: #5a6268;

        }

        

        .btn-danger {

            background: #dc3545;

        }

        

        .btn-danger:hover {

            background: #c82333;

        }

        

        /* Tasks */

        .task-item {

            background: #f8f9fa;

            padding: 1rem;

            border-radius: 8px;

            margin-bottom: 0.5rem;

            display: flex;

            align-items: center;

            gap: 0.75rem;

            transition: all 0.3s ease;

            cursor: pointer;

        }

        

        .task-item:active {

            transform: scale(0.98);

        }

        

        .task-item.completed {

            opacity: 0.6;

        }

        

        .task-item.completed .task-text {

            text-decoration: line-through;

            color: #6c757d;

        }

        

        .task-checkbox {

            width: 24px;

            height: 24px;

            border: 2px solid #4CAF50;

            border-radius: 4px;

            cursor: pointer;

            display: flex;

            align-items: center;

            justify-content: center;

            transition: all 0.3s ease;

            flex-shrink: 0;

        }

        

        .task-checkbox.checked {

            background: #4CAF50;

        }

        

        .task-checkbox.checked::after {

            content: '✓';

            color: white;

            font-weight: bold;

        }

        

        .task-text {

            flex: 1;

            font-size: 1rem;

        }

        

        .task-delete {

            background: #dc3545;

            color: white;

            border: none;

            padding: 0.4rem 0.8rem;

            border-radius: 4px;

            font-size: 0.85rem;

        }

        

        .task-stats {

            background: #e9ecef;

            padding: 0.75rem;

            border-radius: 8px;

            margin-bottom: 1rem;

            text-align: center;

            font-size: 0.9rem;

            color: #666;

        }

        

        /* Agenda */

        .event-item {

            background: #f8f9fa;

            padding: 1rem;

            border-radius: 8px;

            margin-bottom: 0.75rem;

            border-left: 4px solid #4CAF50;

            transition: all 0.3s ease;

        }

        

        .event-item:active {

            transform: scale(0.98);

        }

        

        .event-time {

            font-weight: 600;

            color: #4CAF50;

            font-size: 0.9rem;

        }

        

        .event-title {

            font-size: 1.1rem;

            margin: 0.25rem 0;

        }

        

        .event-date {

            font-size: 0.85rem;

            color: #6c757d;

        }

        

        .event-alerts {

            margin-top: 0.5rem;

            display: flex;

            gap: 0.5rem;

            align-items: center;

            font-size: 0.85rem;

        }

        

        .alert-checkbox {

            margin-right: 0.25rem;

        }

        

        /* Calculator */

        .calculator {

            max-width: 350px;

            margin: 0 auto;

            background: #f8f9fa;

            padding: 1rem;

            border-radius: 12px;

        }

        

        .calc-display {

            background: #333;

            color: white;

            padding: 1rem;

            text-align: right;

            font-size: 1.8rem;

            border-radius: 8px;

            margin-bottom: 1rem;

            min-height: 60px;

            word-wrap: break-word;

            overflow-wrap: break-word;

        }

        

        .calc-buttons {

            display: grid;

            grid-template-columns: repeat(4, 1fr);

            gap: 0.5rem;

        }

        

        .calc-btn {

            padding: 1.2rem;

            font-size: 1.2rem;

            border-radius: 8px;

            background: white;

            border: 1px solid #ddd;

            transition: all 0.2s ease;

        }

        

        .calc-btn:active {

            transform: scale(0.95);

            background: #e9ecef;

        }

        

        .calc-btn.operator {

            background: #4CAF50;

            color: white;

            border: none;

        }

        

        .calc-btn.equals {

            background: #2196F3;

            color: white;

            grid-column: span 2;

            border: none;

        }

        

        .calc-btn.clear {

            background: #dc3545;

            color: white;

            border: none;

        }

        

        /* Weather */

        .weather-container {

            text-align: center;

            padding: 2rem 0;

        }

        

        .weather-info {

            background: #f8f9fa;

            padding: 2rem;

            border-radius: 12px;

            margin-top: 1rem;

        }

        

        .weather-temp {

            font-size: 3rem;

            font-weight: 300;

            color: #4CAF50;

            margin: 1rem 0;

        }

        

        .weather-desc {

            font-size: 1.2rem;

            color: #666;

            text-transform: capitalize;

        }

        

        .weather-details {

            display: grid;

            grid-template-columns: repeat(2, 1fr);

            gap: 1rem;

            margin-top: 1.5rem;

        }

        

        .weather-detail {

            background: white;

            padding: 1rem;

            border-radius: 8px;

        }

        

        .weather-detail-label {

            font-size: 0.85rem;

            color: #6c757d;

        }

        

        .weather-detail-value {

            font-size: 1.1rem;

            font-weight: 600;

            color: #333;

        }

        

        /* Notes */

        .note-item {

            background: #f8f9fa;

            padding: 1rem;

            border-radius: 8px;

            margin-bottom: 0.75rem;

            cursor: pointer;

            transition: all 0.3s ease;

        }

        

        .note-item:active {

            transform: scale(0.98);

        }

        

        .note-title {

            font-weight: 600;

            font-size: 1.1rem;

            margin-bottom: 0.25rem;

        }

        

        .note-content {

            color: #666;

            font-size: 0.9rem;

            margin-bottom: 0.25rem;

            white-space: pre-wrap; /* Show line breaks */

            word-break: break-word;

        }

        

        .note-date {

            font-size: 0.8rem;

            color: #6c757d;

        }

        

        .note-form {

            background: #f8f9fa;

            padding: 1rem;

            border-radius: 8px;

            margin-bottom: 1rem;

        }

        

        .note-form textarea {

            min-height: 120px;

            resize: vertical;

        }

        

        /* Timer */

        .timer-display {

            text-align: center;

            font-size: 4rem;

            font-weight: 300;

            color: #4CAF50;

            margin: 2rem 0;

            font-family: 'Courier New', monospace;

        }

        

        .timer-controls {

            display: flex;

            justify-content: center;

            gap: 1rem;

            margin-bottom: 2rem;

            flex-wrap: wrap;

        }

        

        .timer-presets {

            display: grid;

            grid-template-columns: repeat(2, 1fr);

            gap: 0.5rem;

            max-width: 300px;

            margin: 0 auto;

        }

        

        .preset-btn {

            background: #e9ecef;

            color: #333;

            padding: 0.75rem;

            font-size: 0.9rem;

        }

        

        .preset-btn:hover {

            background: #dee2e6;

        }

        

        /* Backup */

        .backup-section {

            background: #f8f9fa;

            padding: 1.5rem;

            border-radius: 8px;

            margin-bottom: 1rem;

        }

        

        .backup-buttons {

            display: flex;

            gap: 1rem;

            justify-content: center;

            flex-wrap: wrap;

        }

        

        /* Responsiveness */

        @media (max-width: 768px) {

            .timer-display {

                font-size: 3rem;

            }

            

            .calculator {

                max-width: 100%;

            }

            

            .event-alert-title {

                font-size: 2.5rem;

            }

            

            .event-alert-event {

                font-size: 1.5rem;

            }

        }

        

        /* Modal */

        .modal {

            display: none;

            position: fixed;

            top: 0;

            left: 0;

            width: 100%;

            height: 100%;

            background: rgba(0,0,0,0.5);

            z-index: 1000;

            align-items: center;

            justify-content: center;

        }

        

        .modal.active {

            display: flex;

        }

        

        .modal-content {

            background: white;

            padding: 1.5rem;

            border-radius: 12px;

            width: 90%;

            max-width: 500px;

            max-height: 80vh;

            display: flex;

            flex-direction: column;

            animation: modalIn 0.3s ease;

        }

        

        @keyframes modalIn {

            from { transform: scale(0.8); opacity: 0; }

            to { transform: scale(1); opacity: 1; }

        }

        

        .modal-header {

            display: flex;

            justify-content: space-between;

            align-items: center;

            margin-bottom: 1rem;

        }

        

        .modal-close {

            background: none;

            color: #666;

            font-size: 1.5rem;

            padding: 0.5rem;

            width: auto;

        }



        .modal-body {

            overflow-y: auto;

            margin-bottom: 1rem;

            white-space: pre-wrap;

        }



        .modal-footer {

            display: flex;

            gap: 0.5rem;

            justify-content: flex-end;

            margin-top: auto; /* Pushes footer to the bottom */

        }

        

        /* PWA Install Prompt */

        .install-prompt {

            position: fixed;

            bottom: 20px;

            left: 50%;

            transform: translateX(-50%);

            background: #333;

            color: white;

            padding: 1rem 1.5rem;

            border-radius: 50px;

            box-shadow: 0 4px 20px rgba(0,0,0,0.3);

            display: none;

            align-items: center;

            gap: 1rem;

            z-index: 1000;

            animation: slideUp 0.5s ease;

        }

        

        @keyframes slideUp {

            from { transform: translate(-50%, 100px); }

            to { transform: translate(-50%, 0); }

        }

        

        .install-prompt.show {

            display: flex;

        }

        

        .loading {

            text-align: center;

            padding: 2rem;

            color: #666;

        }



        .spinner {

            border: 4px solid rgba(0, 0, 0, 0.1);

            width: 36px;

            height: 36px;

            border-radius: 50%;

            border-left-color: #4CAF50;

            animation: spin 1s ease infinite;

            margin: 20px auto;

        }



        @keyframes spin {

            0% { transform: rotate(0deg); }

            100% { transform: rotate(360deg); }

        }

        

        .error {

            background: #f8d7da;

            color: #721c24;

            padding: 1rem;

            border-radius: 8px;

            margin-bottom: 1rem;

        }

    </style>

</head>

<body>

    <div class="container">

        <header>

            <h1>📋 Meu Planejador</h1>

        </header>

        

        <nav class="nav-tabs">

            <button class="nav-tab active" data-tab="tasks">📝 Tarefas</button>

            <button class="nav-tab" data-tab="calendar">📅 Agenda</button>

            <button class="nav-tab" data-tab="calculator">🧮 Calculadora</button>

            <button class="nav-tab" data-tab="weather">🌤️ Clima</button>

            <button class="nav-tab" data-tab="notes">📋 Notas</button>

            <button class="nav-tab" data-tab="timer">⏱️ Timer</button>

            <button class="nav-tab" data-tab="backup">💾 Backup</button>

        </nav>

        

        <div class="content">

            <!-- Tasks -->

            <div id="tasks" class="tab-content active">

                <div class="task-stats" id="taskStats">

                    Pendentes: 0 | Concluídas: 0

                </div>

                <div class="input-group">

                    <input type="text" id="taskInput" placeholder="Nova tarefa..." />

                    <button onclick="addTask()">Adicionar</button>

                </div>

                 <div class="input-group">

                    <button class="gemini-btn" onclick="planTasksWithGemini()" style="width: 100%;">✨ Planejar Tarefas com IA</button>

                </div>

                <div id="taskList"></div>

            </div>

            

            <!-- Calendar -->

            <div id="calendar" class="tab-content">

                <div class="input-group">

                    <input type="text" id="eventTitle" placeholder="Título do evento" />

                </div>

                <div class="input-group">

                    <input type="datetime-local" id="eventDateTime" />

                    <button onclick="addEvent()">Adicionar</button>

                </div>

                <h3 style="margin-top: 1.5rem; margin-bottom: 1rem;">Opções de Alerta:</h3>

                <div style="background: #f8f9fa; padding: 1rem; border-radius: 8px; margin-bottom: 1rem;">

                    <label style="display: flex; align-items: center; margin-bottom: 0.5rem;">

                        <input type="checkbox" id="alertOnTime" checked style="margin-right: 0.5rem;">

                        Alertar na hora exata

                    </label>

                    <label style="display: flex; align-items: center; margin-bottom: 0.5rem;">

                        <input type="checkbox" id="alert3Min" checked style="margin-right: 0.5rem;">

                        Alertar 3 minutos antes

                    </label>

                    <label style="display: flex; align-items: center;">

                        <input type="checkbox" id="alert15Min" style="margin-right: 0.5rem;">

                        Alertar 15 minutos antes

                    </label>

                </div>

                <div id="eventList"></div>

            </div>

            

            <!-- Calculator -->

            <div id="calculator" class="tab-content">

                <div class="calculator">

                    <div class="calc-display" id="calcDisplay">0</div>

                    <div class="calc-buttons">

                        <button class="calc-btn clear" onclick="clearCalc()">C</button>

                        <button class="calc-btn operator" onclick="appendCalc('/')">/</button>

                        <button class="calc-btn operator" onclick="appendCalc('*')">×</button>

                        <button class="calc-btn" onclick="deleteCalc()">←</button>

                        

                        <button class="calc-btn" onclick="appendCalc('7')">7</button>

                        <button class="calc-btn" onclick="appendCalc('8')">8</button>

                        <button class="calc-btn" onclick="appendCalc('9')">9</button>

                        <button class="calc-btn operator" onclick="appendCalc('-')">-</button>

                        

                        <button class="calc-btn" onclick="appendCalc('4')">4</button>

                        <button class="calc-btn" onclick="appendCalc('5')">5</button>

                        <button class="calc-btn" onclick="appendCalc('6')">6</button>

                        <button class="calc-btn operator" onclick="appendCalc('+')">+</button>

                        

                        <button class="calc-btn" onclick="appendCalc('1')">1</button>

                        <button class="calc-btn" onclick="appendCalc('2')">2</button>

                        <button class="calc-btn" onclick="appendCalc('3')">3</button>

                        <button class="calc-btn" onclick="appendCalc('.')">.</button>

                        

                        <button class="calc-btn" onclick="appendCalc('0')">0</button>

                        <button class="calc-btn" onclick="appendCalc('00')">00</button>

                        <button class="calc-btn equals" onclick="calculate()">=</button>

                    </div>

                </div>

            </div>

            

            <!-- Weather -->

            <div id="weather" class="tab-content">

                <div class="weather-container">

                    <button onclick="getWeather()">🔄 Atualizar Clima</button>

                    <div id="weatherInfo" class="weather-info">

                        <div class="loading">Clique em "Atualizar Clima" para começar.</div>

                    </div>

                </div>

            </div>

            

            <!-- Notes -->

            <div id="notes" class="tab-content">

                <div class="note-form">

                    <input type="text" id="noteTitle" placeholder="Título da nota" />

                    <textarea id="noteContent" placeholder="Conteúdo da nota..."></textarea>

                    <button onclick="addNote()">Salvar Nota</button>

                </div>

                <div id="notesList"></div>

            </div>

            

            <!-- Timer -->

            <div id="timer" class="tab-content">

                <div class="timer-display" id="timerDisplay">00:00:00</div>

                <div class="timer-controls">

                    <button id="startTimer" onclick="startTimer()">▶️ Iniciar</button>

                    <button id="pauseTimer" onclick="pauseTimer()" style="display:none">⏸️ Pausar</button>

                    <button onclick="resetTimer()">🔄 Resetar</button>

                </div>

                <div class="timer-presets">

                    <button class="preset-btn" onclick="setTimer(1)">1 min</button>

                    <button class="preset-btn" onclick="setTimer(5)">5 min</button>

                    <button class="preset-btn" onclick="setTimer(10)">10 min</button>

                    <button class="preset-btn" onclick="setTimer(15)">15 min</button>

                </div>

            </div>

            

            <!-- Backup -->

            <div id="backup" class="tab-content">

                <div class="backup-section">

                    <h3>📤 Exportar Dados</h3>

                    <p>Salve todos os seus dados em um arquivo para mantê-los seguros.</p>

                    <button onclick="exportData()">Exportar Dados</button>

                </div>

                <div class="backup-section">

                    <h3>📥 Importar Dados</h3>

                    <p>Restaure seus dados de um arquivo de backup. (Isso substituirá os dados atuais)</p>

                    <input type="file" id="importFile" accept=".json" style="display:none" onchange="importData(event)" />

                    <button onclick="document.getElementById('importFile').click()">Importar Dados</button>

                </div>

            </div>

        </div>

    </div>

    

    <!-- Generic Modal -->

    <div class="modal" id="modal">

        <div class="modal-content">

            <div class="modal-header">

                <h3 id="modalTitle"></h3>

                <button class="modal-close" onclick="closeModal()">×</button>

            </div>

            <div class="modal-body" id="modalBody"></div>

            <div class="modal-footer" id="modalFooter"></div>

        </div>

    </div>

    

    <!-- Full-screen Event Alert -->

    <div class="event-alert-overlay" id="eventAlertOverlay">

        <div class="event-alert-content">

            <div class="event-alert-icon">⏰</div>

            <div class="event-alert-title">HORA DO COMPROMISSO!</div>

            <div class="event-alert-event" id="alertEventTitle"></div>

            <button class="event-alert-dismiss" onclick="dismissEventAlert()">OK, ENTENDI!</button>

        </div>

    </div>

    

    <!-- PWA Install Prompt -->

    <div class="install-prompt" id="installPrompt">

        <span>Instalar o aplicativo?</span>

        <button onclick="installPWA()">Instalar</button>

    </div>

    

    <script>

        // --- GLOBAL STATE & VARIABLES ---

        let appData = {

            tasks: [],

            events: [],

            notes: [],

            weather: null,

            lastWeatherUpdate: null

        };

        

        let timerInterval = null;

        let timerSeconds = 0;

        let timerMode = 'stopwatch';

        let countdownTime = 0;

        

        let calcDisplay = '0';

        let calcHistory = [];

        

        let deferredPrompt;

        let alertSound = null;

        let eventCheckInterval = null;



        // --- INITIALIZATION ---

        document.addEventListener('DOMContentLoaded', function() {

            loadData();

            updateAllViews();

            setupEventListeners();

            setupEventChecking();

            requestNotificationPermission();

            initializeAlertSound();

            

            window.addEventListener('beforeinstallprompt', (e) => {

                e.preventDefault();

                deferredPrompt = e;

                document.getElementById('installPrompt').classList.add('show');

            });

            

            document.addEventListener('visibilitychange', function() {

                if (!document.hidden) {

                    setupEventChecking();

                }

            });

        });



        function initializeAlertSound() {

            if (window.AudioContext || window.webkitAudioContext) {

                const AudioContext = window.AudioContext || window.webkitAudioContext;

                alertSound = new AudioContext();

            }

        }



        function requestNotificationPermission() {

            if ('Notification' in window && Notification.permission === 'default') {

                Notification.requestPermission();

            }

        }



        function setupEventListeners() {

            document.querySelectorAll('.nav-tab').forEach(tab => {

                tab.addEventListener('click', function() {

                    switchTab(this.dataset.tab);

                });

            });

            

            document.getElementById('taskInput').addEventListener('keypress', function(e) {

                if (e.key === 'Enter') addTask();

            });

            

            document.getElementById('modal').addEventListener('click', function(e) {

                if (e.target === this) closeModal();

            });

        }



        // --- NAVIGATION ---

        function switchTab(tabName) {

            document.querySelectorAll('.nav-tab').forEach(tab => tab.classList.remove('active'));

            document.querySelectorAll('.tab-content').forEach(content => content.classList.remove('active'));

            

            document.querySelector(`[data-tab="${tabName}"]`).classList.add('active');

            document.getElementById(tabName).classList.add('active');

            

            if (tabName === 'weather' && (!appData.lastWeatherUpdate || Date.now() - appData.lastWeatherUpdate > 600000)) {

                getWeather();

            }

        }



        // --- TASKS ---

        function addTask() {

            const input = document.getElementById('taskInput');

            const text = input.value.trim();

            if (!text) return;

            

            const task = {

                id: Date.now(),

                text: text,

                completed: false,

                createdAt: new Date().toISOString()

            };

            

            appData.tasks.push(task);

            input.value = '';

            saveData();

            renderTasks();

        }



        function toggleTask(id) {

            const task = appData.tasks.find(t => t.id === id);

            if (task) {

                task.completed = !task.completed;

                saveData();

                renderTasks();

            }

        }



        function deleteTask(id) {

            appData.tasks = appData.tasks.filter(t => t.id !== id);

            saveData();

            renderTasks();

        }



        function renderTasks() {

            const container = document.getElementById('taskList');

            const stats = document.getElementById('taskStats');

            

            const pending = appData.tasks.filter(t => !t.completed).length;

            const completed = appData.tasks.filter(t => t.completed).length;

            stats.textContent = `Pendentes: ${pending} | Concluídas: ${completed}`;

            

            container.innerHTML = appData.tasks

                .sort((a, b) => a.completed - b.completed || b.id - a.id)

                .map(task => `

                    <div class="task-item ${task.completed ? 'completed' : ''}" onclick="toggleTask(${task.id})">

                        <div class="task-checkbox ${task.completed ? 'checked' : ''}"></div>

                        <span class="task-text">${escapeHtml(task.text)}</span>

                        <button class="task-delete" onclick="event.stopPropagation(); deleteTask(${task.id})">×</button>

                    </div>

                `).join('');

        }



        // --- CALENDAR & ALERTS ---

        function addEvent() {

            const title = document.getElementById('eventTitle').value.trim();

            const dateTime = document.getElementById('eventDateTime').value;

            if (!title || !dateTime) return;

            

            const event = {

                id: Date.now(),

                title: title,

                dateTime: new Date(dateTime).toISOString(),

                alerts: {

                    onTime: document.getElementById('alertOnTime').checked,

                    before3Min: document.getElementById('alert3Min').checked,

                    before15Min: document.getElementById('alert15Min').checked

                },

                notified: { onTime: false, before3Min: false, before15Min: false }

            };

            

            appData.events.push(event);

            document.getElementById('eventTitle').value = '';

            document.getElementById('eventDateTime').value = '';

            saveData();

            renderEvents();

        }



        function deleteEvent(id) {

            appData.events = appData.events.filter(e => e.id !== id);

            saveData();

            renderEvents();

        }



        function renderEvents() {

            const container = document.getElementById('eventList');

            const now = new Date();

            

            container.innerHTML = appData.events

                .filter(event => new Date(event.dateTime) > now) // Only show upcoming events

                .sort((a, b) => new Date(a.dateTime) - new Date(b.dateTime))

                .map(event => {

                    const eventDate = new Date(event.dateTime);

                    const alertsText = [];

                    if (event.alerts?.onTime) alertsText.push('Na hora');

                    if (event.alerts?.before3Min) alertsText.push('3 min antes');

                    if (event.alerts?.before15Min) alertsText.push('15 min antes');

                    

                    return `

                        <div class="event-item">

                            <div class="event-time">${eventDate.toLocaleTimeString('pt-BR', { hour: '2-digit', minute: '2-digit' })}</div>

                            <div class="event-title">${escapeHtml(event.title)}</div>

                            <div class="event-date">${eventDate.toLocaleDateString('pt-BR', {weekday: 'long', day: '2-digit', month: 'long'})}</div>

                            ${alertsText.length > 0 ? `<div class="event-alerts">🔔 ${alertsText.join(', ')}</div>` : ''}

                            <button class="task-delete" style="float: right;" onclick="deleteEvent(${event.id})">Excluir</button>

                        </div>

                    `;

                }).join('');

        }



        function setupEventChecking() {

            if (eventCheckInterval) clearInterval(eventCheckInterval);

            eventCheckInterval = setInterval(checkEventAlerts, 10000); // Check every 10 seconds

            checkEventAlerts();

        }



        function checkEventAlerts() {

            const now = new Date();

            appData.events.forEach(event => {

                if (!event.alerts) return;

                const eventTime = new Date(event.dateTime);

                const timeDiff = (eventTime - now) / 1000;

                

                if (event.alerts.before15Min && !event.notified.before15Min && timeDiff > 0 && timeDiff <= 900) {

                    event.notified.before15Min = true;

                    showNotification(event.title, 'em 15 minutos');

                    saveData();

                }

                if (event.alerts.before3Min && !event.notified.before3Min && timeDiff > 0 && timeDiff <= 180) {

                    event.notified.before3Min = true;

                    showNotification(event.title, 'em 3 minutos');

                    saveData();

                }

                if (event.alerts.onTime && !event.notified.onTime && Math.abs(timeDiff) <= 30) {

                    event.notified.onTime = true;

                    showEventAlert(event.title);

                    saveData();

                }

            });

        }



        function showNotification(eventTitle, timeText) {

            playAlertSound();

            if ('Notification' in window && Notification.permission === 'granted') {

                new Notification('📅 Lembrete de Evento', {

                    body: `${eventTitle} ${timeText}!`,

                    icon: 'data:image/png;base64,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',

                    requireInteraction: true

                });

            }

            if ('vibrate' in navigator) navigator.vibrate([200, 100, 200]);

        }



        function showEventAlert(eventTitle) {

            playAlertSoundContinuous();

            document.getElementById('alertEventTitle').textContent = eventTitle;

            document.getElementById('eventAlertOverlay').classList.add('show');

            if ('vibrate' in navigator) navigator.vibrate([500, 250, 500, 250, 500]);

        }



        function dismissEventAlert() {

            document.getElementById('eventAlertOverlay').classList.remove('show');

            stopAlertSound();

        }



        function playAlertSound() {

            if (!alertSound) return;

            const oscillator = alertSound.createOscillator();

            const gainNode = alertSound.createGain();

            oscillator.connect(gainNode);

            gainNode.connect(alertSound.destination);

            oscillator.frequency.value = 800;

            gainNode.gain.setValueAtTime(0.3, alertSound.currentTime);

            oscillator.start();

            oscillator.stop(alertSound.currentTime + 0.3);

        }



        let continuousAlertInterval = null;

        function playAlertSoundContinuous() {

            stopAlertSound();

            continuousAlertInterval = setInterval(playAlertSound, 500);

        }



        function stopAlertSound() {

            if (continuousAlertInterval) clearInterval(continuousAlertInterval);

            continuousAlertInterval = null;

        }



        // --- CALCULATOR ---

        function appendCalc(value) {

            if (calcDisplay === '0' && value !== '.') calcDisplay = '';

            if (calcDisplay === 'Erro') calcDisplay = '';

            calcDisplay += value;

            updateCalcDisplay();

        }



        function clearCalc() {

            calcDisplay = '0';

            updateCalcDisplay();

        }



        function deleteCalc() {

            calcDisplay = calcDisplay.length > 1 ? calcDisplay.slice(0, -1) : '0';

            updateCalcDisplay();

        }



        function safeCalculate(expression) {

            const sanitized = expression.replace(/×/g, '*').replace(/÷/g, '/');

            if (!/^[0-9+\-*/.() ]+$/.test(sanitized)) return 'Erro';

            try {

                return new Function('return ' + sanitized)();

            } catch (e) {

                return 'Erro';

            }

        }



        function calculate() {

            const result = safeCalculate(calcDisplay);

            if (result === 'Erro') {

                calcDisplay = 'Erro';

                updateCalcDisplay();

                setTimeout(() => {

                    if (calcDisplay === 'Erro') clearCalc();

                }, 1500);

            } else {

                calcHistory.push(`${calcDisplay} = ${result}`);

                calcDisplay = result.toString();

                updateCalcDisplay();

            }

        }



        function updateCalcDisplay() {

            document.getElementById('calcDisplay').textContent = calcDisplay;

        }



        // --- WEATHER ---

        function getWeather() {

            const weatherInfo = document.getElementById('weatherInfo');

            weatherInfo.innerHTML = '<div class="loading">Obtendo localização...</div>';

            if (navigator.geolocation) {

                navigator.geolocation.getCurrentPosition(

                    position => fetchWeatherData(position.coords),

                    () => {

                        weatherInfo.innerHTML = '<div class="error">Erro ao obter localização. Verifique as permissões.</div>';

                    }

                );

            } else {

                weatherInfo.innerHTML = '<div class="error">Geolocalização não suportada.</div>';

            }

        }



        function fetchWeatherData(coords) {

            const weatherInfo = document.getElementById('weatherInfo');

            weatherInfo.innerHTML = '<div class="loading">Carregando dados do clima...</div>';

            

            // This is a simulation. For production, replace with a real weather API call.

            setTimeout(() => {

                const weatherData = {

                    temp: Math.round(15 + Math.random() * 15),

                    description: ['Ensolarado', 'Parcialmente nublado', 'Nublado', 'Chuva leve'][Math.floor(Math.random() * 4)],

                    humidity: Math.round(40 + Math.random() * 50),

                    windSpeed: Math.round(5 + Math.random() * 15),

                    location: 'Sua Localização'

                };

                appData.weather = weatherData;

                appData.lastWeatherUpdate = Date.now();

                saveData();

                renderWeather();

            }, 1000);

        }



        function renderWeather() {

            const weatherInfo = document.getElementById('weatherInfo');

            const data = appData.weather;

            if (!data) return;

            weatherInfo.innerHTML = `

                <h3>${data.location}</h3>

                <div class="weather-temp">${data.temp}°C</div>

                <div class="weather-desc">${data.description}</div>

                <div class="weather-details">

                    <div class="weather-detail">

                        <div class="weather-detail-label">Umidade</div>

                        <div class="weather-detail-value">${data.humidity}%</div>

                    </div>

                    <div class="weather-detail">

                        <div class="weather-detail-label">Vento</div>

                        <div class="weather-detail-value">${data.windSpeed} km/h</div>

                    </div>

                </div>

            `;

        }



        // --- NOTES ---

        function addNote() {

            const title = document.getElementById('noteTitle').value.trim();

            const content = document.getElementById('noteContent').value.trim();

            if (!title && !content) return;

            

            const note = {

                id: Date.now(),

                title: title || 'Sem título',

                content: content,

                createdAt: new Date().toISOString()

            };

            

            appData.notes.push(note);

            document.getElementById('noteTitle').value = '';

            document.getElementById('noteContent').value = '';

            saveData();

            renderNotes();

        }



        function deleteNote(id) {

            appData.notes = appData.notes.filter(n => n.id !== id);

            saveData();

            renderNotes();

        }



        function editNote(id) {

            const note = appData.notes.find(n => n.id === id);

            if (!note) return;

            

            const body = `

                <input type="text" id="editNoteTitle" value="${escapeHtml(note.title)}" placeholder="Título da nota" style="width: 100%; margin-bottom: 0.5rem;" />

                <textarea id="editNoteContent" placeholder="Conteúdo da nota..." style="width: 100%; min-height: 150px;">${escapeHtml(note.content)}</textarea>

            `;

            const footer = `

                <button class="gemini-btn" onclick="summarizeNoteWithGemini(${id})">✨ Resumir</button>

                <button class="gemini-btn" onclick="continueNoteWithGemini(${id})">✨ Continuar</button>

                <button onclick="saveEditedNote(${id})">Salvar</button>

                <button class="btn-secondary" onclick="closeModal()">Cancelar</button>

            `;

            openModal('Editar Nota', body, footer);

        }



        function saveEditedNote(id) {

            const note = appData.notes.find(n => n.id === id);

            if (!note) return;

            

            note.title = document.getElementById('editNoteTitle').value.trim() || 'Sem título';

            note.content = document.getElementById('editNoteContent').value.trim();

            saveData();

            renderNotes();

            closeModal();

        }



        function renderNotes() {

            const container = document.getElementById('notesList');

            container.innerHTML = appData.notes

                .sort((a, b) => new Date(b.createdAt) - new Date(a.createdAt))

                .map(note => `

                    <div class="note-item" onclick="editNote(${note.id})">

                        <div class="note-title">${escapeHtml(note.title)}</div>

                        <div class="note-content">${escapeHtml(note.content.substring(0, 100))}${note.content.length > 100 ? '...' : ''}</div>

                        <div class="note-date">${new Date(note.createdAt).toLocaleString('pt-BR')}</div>

                        <button class="btn-danger" style="float: right;" onclick="event.stopPropagation(); deleteNote(${note.id})">Excluir</button>

                    </div>

                `).join('');

        }



        // --- TIMER ---

        function startTimer() {

            if (timerInterval) return;

            document.getElementById('startTimer').style.display = 'none';

            document.getElementById('pauseTimer').style.display = 'inline-block';

            

            timerInterval = setInterval(() => {

                if (timerMode === 'countdown') {

                    timerSeconds--;

                    if (timerSeconds <= 0) {

                        timerSeconds = 0;

                        pauseTimer();

                        playTimerAlert();

                    }

                } else {

                    timerSeconds++;

                }

                updateTimerDisplay();

            }, 1000);

        }



        function pauseTimer() {

            clearInterval(timerInterval);

            timerInterval = null;

            document.getElementById('startTimer').style.display = 'inline-block';

            document.getElementById('pauseTimer').style.display = 'none';

        }



        function resetTimer() {

            pauseTimer();

            timerSeconds = timerMode === 'countdown' ? countdownTime : 0;

            updateTimerDisplay();

        }



        function setTimer(minutes) {

            pauseTimer();

            timerMode = 'countdown';

            countdownTime = minutes * 60;

            timerSeconds = countdownTime;

            updateTimerDisplay();

        }



        function updateTimerDisplay() {

            const h = Math.floor(timerSeconds / 3600).toString().padStart(2, '0');

            const m = Math.floor((timerSeconds % 3600) / 60).toString().padStart(2, '0');

            const s = (timerSeconds % 60).toString().padStart(2, '0');

            document.getElementById('timerDisplay').textContent = `${h}:${m}:${s}`;

        }



        function playTimerAlert() {

            playAlertSound();

            if ('Notification' in window && Notification.permission === 'granted') {

                new Notification('Timer Finalizado!', { body: 'O tempo acabou!' });

            }

        }



        // --- BACKUP & DATA ---

        function exportData() {

            const dataStr = JSON.stringify(appData, null, 2);

            const dataBlob = new Blob([dataStr], { type: 'application/json' });

            const url = URL.createObjectURL(dataBlob);

            

            const a = document.createElement('a');

            a.href = url;

            a.download = `meu-planejador-backup-${new Date().toISOString().split('T')[0]}.json`;

            document.body.appendChild(a);

            a.click();

            document.body.removeChild(a);

            URL.revokeObjectURL(url);

            

            openModal('Sucesso', '<p>Dados exportados com sucesso!</p>', '<button onclick="closeModal()">OK</button>');

        }



        function importData(event) {

            const file = event.target.files[0];

            if (!file) return;

            

            const reader = new FileReader();

            reader.onload = function(e) {

                const dataString = e.target.result;

                try {

                    JSON.parse(dataString); // Validate JSON

                    const body = '<p>Isso substituirá todos os dados atuais. Deseja continuar?</p>';

                    const footer = `

                        <button onclick="performImport(JSON.parse(decodeURIComponent('${encodeURIComponent(dataString)}')))">Confirmar</button>

                        <button class="btn-secondary" onclick="closeModal()">Cancelar</button>

                    `;

                    openModal('Confirmar Importação', body, footer);

                } catch (error) {

                    openModal('Erro', '<p>Arquivo de backup inválido.</p>', '<button onclick="closeModal()">OK</button>');

                }

            };

            reader.readAsText(file);

            event.target.value = ''; // Reset file input

        }



        function performImport(importedData) {

            appData = { ...appData, ...importedData };

            saveData();

            updateAllViews();

            closeModal();

            openModal('Sucesso', '<p>Dados importados com sucesso!</p>', '<button onclick="closeModal()">OK</button>');

        }



        function saveData() {

            localStorage.setItem('planejadorData', JSON.stringify(appData));

        }



        function loadData() {

            const saved = localStorage.getItem('planejadorData');

            if (saved) appData = JSON.parse(saved);

        }



        // --- GEMINI API FEATURES ---



        async function callGemini(prompt) {

            const apiKey = ""; // Leave empty, will be handled by the environment

            const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${apiKey}`;



            const payload = {

                contents: [{

                    role: "user",

                    parts: [{ text: prompt }]

                }]

            };



            try {

                const response = await fetch(apiUrl, {

                    method: 'POST',

                    headers: { 'Content-Type': 'application/json' },

                    body: JSON.stringify(payload)

                });



                if (!response.ok) {

                    throw new Error(`HTTP error! status: ${response.status}`);

                }



                const result = await response.json();

                

                if (result.candidates && result.candidates.length > 0 &&

                    result.candidates[0].content && result.candidates[0].content.parts &&

                    result.candidates[0].content.parts.length > 0) {

                    return result.candidates[0].content.parts[0].text;

                } else {

                    console.error("Gemini API response format is unexpected:", result);

                    // Check for blocked content

                    if (result.candidates && result.candidates[0] && result.candidates[0].finishReason === 'SAFETY') {

                         return "A resposta foi bloqueada por motivos de segurança.";

                    }

                    return "Não foi possível obter uma resposta da IA.";

                }

            } catch (error) {

                console.error("Error calling Gemini API:", error);

                return "Erro ao conectar com a IA. Verifique sua conexão.";

            }

        }



        async function planTasksWithGemini() {

            const pendingTasks = appData.tasks.filter(t => !t.completed);

            if (pendingTasks.length === 0) {

                openModal('Nenhuma Tarefa', '<p>Adicione algumas tarefas pendentes antes de usar o planejador de IA.</p>', '<button onclick="closeModal()">OK</button>');

                return;

            }



            const taskList = pendingTasks.map(t => `- ${t.text}`).join('\n');

            const prompt = `Como um assistente de produtividade, crie um plano de ação detalhado para as seguintes tarefas:\n\n${taskList}\n\nDivida o plano em etapas claras e acionáveis.`;



            openModal('✨ Planejando com IA...', '<div class="spinner"></div><p>Aguarde, a IA está criando seu plano de ação...</p>', '');

            

            const plan = await callGemini(prompt);

            

            const body = `<p><strong>Plano de Ação Sugerido:</strong></p><pre style="white-space: pre-wrap; word-wrap: break-word; background: #f8f9fa; padding: 1rem; border-radius: 8px;">${escapeHtml(plan)}</pre>`;

            const footer = '<button onclick="closeModal()">Fechar</button>';

            openModal('✨ Plano de Ação da IA', body, footer);

        }



        async function summarizeNoteWithGemini(noteId) {

            const note = appData.notes.find(n => n.id === noteId);

            if (!note || !note.content) return;



            const prompt = `Resuma o seguinte texto em um ou dois parágrafos curtos:\n\n---\n${note.content}\n---`;

            

            openModal('✨ Resumindo com IA...', '<div class="spinner"></div><p>Aguarde, a IA está processando sua nota...</p>', '');



            const summary = await callGemini(prompt);



            const body = `<p><strong>Resumo da Nota:</strong></p><p>${escapeHtml(summary)}</p>`;

            const footer = '<button onclick="closeModal()">Fechar</button>';

            openModal('✨ Resumo da IA', body, footer);

        }



        async function continueNoteWithGemini(noteId) {

            const noteContentElement = document.getElementById('editNoteContent');

            if (!noteContentElement) return;



            const currentText = noteContentElement.value;

            if (!currentText) return;



            const prompt = `Continue escrevendo o texto a seguir, adicionando um ou dois parágrafos que sigam o mesmo tom e estilo:\n\n---\n${currentText}\n---`;



            const button = event.target;

            button.disabled = true;

            button.innerHTML = '✨ Escrevendo...';



            const continuation = await callGemini(prompt);



            noteContentElement.value += `\n\n${continuation}`;



            button.disabled = false;

            button.innerHTML = '✨ Continuar';

        }





        // --- UTILITIES & MODAL ---

        function escapeHtml(text) {

            if (typeof text !== 'string') return '';

            const div = document.createElement('div');

            div.textContent = text;

            return div.innerHTML;

        }

        

        function openModal(title, bodyHtml, footerHtml) {

            document.getElementById('modalTitle').textContent = title;

            document.getElementById('modalBody').innerHTML = bodyHtml;

            document.getElementById('modalFooter').innerHTML = footerHtml;

            document.getElementById('modal').classList.add('active');

        }



        function closeModal() {

            document.getElementById('modal').classList.remove('active');

        }

        

        function updateAllViews() {

            renderTasks();

            renderEvents();

            renderNotes();

            updateTimerDisplay();

            updateCalcDisplay();

            if (appData.weather) renderWeather();

        }



        // --- PWA ---

        function installPWA() {

            if (deferredPrompt) {

                deferredPrompt.prompt();

                deferredPrompt.userChoice.then(() => {

                    deferredPrompt = null;

                    document.getElementById('installPrompt').classList.remove('show');

                });

            }

        }

    </script>

</body>

</html>
