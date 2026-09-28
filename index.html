<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grafischer Taschenrechner</title>

    <!-- Google Fonts für eine moderne Typografie -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

    <style>
        /* 
         * ==========================================
         * 1. CSS STYLES (Das Design & Layout)
         * ==========================================
         */

        /* Grundeinstellungen für die gesamte Seite */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Inter', sans-serif;
            user-select: none; /* Verhindert ungewolltes Markieren von Text */
        }

        body {
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
            color: #f8fafc;
        }

        /* Container für den Rechner */
        .calculator {
            background-color: #1e293b;
            width: 100%;
            max-width: 360px;
            border-radius: 24px;
            padding: 24px;
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.4),
                        0 0 0 1px rgba(255, 255, 255, 0.1);
        }

        /* Titelzeile */
        .header {
            text-align: center;
            margin-bottom: 20px;
        }

        .header h1 {
            font-size: 1.25rem;
            font-weight: 600;
            color: #94a3b8;
            letter-spacing: 0.5px;
        }

        /* DISPLAY-BEREICH */
        .display-container {
            background-color: #0f172a;
            border-radius: 16px;
            padding: 16px 20px;
            margin-bottom: 20px;
            text-align: right;
            box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.5);
            word-wrap: break-word;
            word-break: break-all;
            min-height: 90px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        /* Vorheriger Ausdruck (kleiner Text oben) */
        .previous-expression {
            color: #64748b;
            font-size: 0.9rem;
            min-height: 1.2rem;
            overflow: hidden;
        }

        /* Aktuelle Eingabe / Ergebnis (großer Text unten) */
        .current-input {
            color: #f8fafc;
            font-size: 2.2rem;
            font-weight: 700;
            line-height: 1.2;
            transition: font-size 0.2s ease;
        }

        /* TASTEN-RASTER (GRID) */
        .buttons-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 12px;
        }

        /* Allgemeine Tasten-Styles */
        button {
            background-color: #334155;
            color: #f8fafc;
            border: none;
            border-radius: 14px;
            padding: 18px 0;
            font-size: 1.25rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.15s ease;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.2);
            outline: none;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        /* Effekte beim Drücken und Hovern */
        button:hover {
            background-color: #475569;
            transform: translateY(-2px);
            box-shadow: 0 6px 12px -2px rgba(0, 0, 0, 0.3);
        }

        button:active {
            transform: translateY(1px);
            box-shadow: 0 2px 4px -1px rgba(0, 0, 0, 0.2);
        }

        /* Spezialtasten: Operatoren (+, -, *, /) */
        button.operator {
            background-color: #3b82f6;
            color: #ffffff;
        }

        button.operator:hover {
            background-color: #60a5fa;
        }

        /* Spezialtaste: Löschen (C, Delete) */
        button.action {
            background-color: #ef4444;
            color: #ffffff;
        }

        button.action:hover {
            background-color: #f87171;
        }

        /* Spezialtaste: Gleichheitszeichen (=) */
        button.equals {
            background-color: #10b981;
            color: #ffffff;
            grid-column: span 2; /* Erstreckt sich über 2 Spalten */
        }

        button.equals:hover {
            background-color: #34d399;
        }

        /* Footer Info für GitHub */
        .footer {
            margin-top: 24px;
            font-size: 0.85rem;
            color: #64748b;
            text-align: center;
        }

        .footer a {
            color: #3b82f6;
            text-decoration: none;
        }

        .footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <!-- 
      ==========================================
      2. HTML STRUKTUR (Das Grundgerüst)
      ==========================================
    -->
    <div class="calculator">
        <div class="header">
            <h1>Taschenrechner</h1>
        </div>

        <!-- Display zur Anzeige der Zahlen und Rechenwege -->
        <div class="display-container">
            <div id="previous-expression" class="previous-expression"></div>
            <div id="current-input" class="current-input">0</div>
        </div>

        <!-- Tastenfeld -->
        <div class="buttons-grid">
            <!-- Reihe 1 -->
            <button class="action" onclick="clearAll()">C</button>
            <button class="action" onclick="deleteLast()">⌫</button>
            <button class="operator" onclick="appendOperator('/')">÷</button>
            <button class="operator" onclick="appendOperator('*')">×</button>

            <!-- Reihe 2 -->
            <button onclick="appendNumber('7')">7</button>
            <button onclick="appendNumber('8')">8</button>
            <button onclick="appendNumber('9')">9</button>
            <button class="operator" onclick="appendOperator('-')">−</button>

            <!-- Reihe 3 -->
            <button onclick="appendNumber('4')">4</button>
            <button onclick="appendNumber('5')">5</button>
            <button onclick="appendNumber('6')">6</button>
            <button class="operator" onclick="appendOperator('+')">+</button>

            <!-- Reihe 4 -->
            <button onclick="appendNumber('1')">1</button>
            <button onclick="appendNumber('2')">2</button>
            <button onclick="appendNumber('3')">3</button>
            <button class="equals" onclick="calculate()">=</button>

            <!-- Reihe 5 -->
            <button onclick="appendNumber('0')" style="grid-column: span 2;">0</button>
            <button onclick="appendDecimal()">.</button>
        </div>
    </div>

    <div class="footer">
        Erstellt für GitHub Pages • Tastatureingabe unterstützt
    </div>

    <!-- 
      ==========================================
      3. JAVASCRIPT LOGIK (Die Funktionsweise)
      ==========================================
    -->
    <script>
        // Referenzen auf die HTML-Elemente für das Display holen
        const currentInputDisplay = document.getElementById('current-input');
        const previousExpressionDisplay = document.getElementById('previous-expression');

        // Status-Variablen zum Speichern der Daten
        let currentInput = '0';      // Die aktuell eingegebene Zahl
        let previousExpression = ''; // Der obere Verlaufstext
        let isCalculated = false;    // Merkt sich, ob gerade ein Ergebnis berechnet wurde

        /**
         * Aktualisiert die Anzeige im HTML basierend auf den JavaScript-Variablen
         */
        function updateDisplay() {
            currentInputDisplay.innerText = currentInput;
            previousExpressionDisplay.innerText = previousExpression;
        }

        /**
         * Fügt eine Zahl (0-9) zur aktuellen Eingabe hinzu
         * @param {string} number - Die anzuhängende Zahl
         */
        function appendNumber(number) {
            // Wenn gerade erst gerechnet wurde, startet eine neue Eingabe
            if (isCalculated) {
                currentInput = number;
                previousExpression = '';
                isCalculated = false;
            } else {
                // Verhindert mehrfache führende Nullen (z. B. "00")
                if (currentInput === '0') {
                    currentInput = number;
                } else {
                    currentInput += number;
                }
            }
            updateDisplay();
        }

        /**
         * Fügt einen Dezimalpunkt hinzu
         */
        function appendDecimal() {
            if (isCalculated) {
                currentInput = '0.';
                previousExpression = '';
                isCalculated = false;
            } else if (!currentInput.includes('.')) {
                currentInput += '.';
            }
            updateDisplay();
        }

        /**
         * Fügt einen Operator (+, -, *, /) hinzu
         * @param {string} op - Der mathematische Operator
         */
        function appendOperator(op) {
            // Falls das Ergebnis gerade berechnet wurde, kann direkt weitergrechnet werden
            if (isCalculated) {
                isCalculated = false;
            }

            // Prüfen, ob das letzte Zeichen in der Eingabe bereits ein Operator ist
            const lastChar = currentInput.slice(-1);
            if (['+', '-', '*', '/'].includes(lastChar)) {
                // Ersetzt den alten Operator durch den neuen
                currentInput = currentInput.slice(0, -1) + op;
            } else {
                currentInput += op;
            }
            updateDisplay();
        }

        /**
         * Löscht die gesamte Eingabe (Clear / C)
         */
        function clearAll() {
            currentInput = '0';
            previousExpression = '';
            isCalculated = false;
            updateDisplay();
        }

        /**
         * Löscht das letzte Zeichen (Backspace / Delete)
         */
        function deleteLast() {
            if (isCalculated) {
                clearAll();
                return;
            }

            if (currentInput.length === 1) {
                currentInput = '0';
            } else {
                currentInput = currentInput.slice(0, -1);
            }
            updateDisplay();
        }

        /**
         * Führt die eigentliche Berechnung durch (=)
         */
        function calculate() {
            try {
                // Speichere den Ausdruck für die obere Zeile
                previousExpression = currentInput.replace(/\*/g, '×').replace(/\//g, '÷') + ' =';
                
                // Ersetze Anzeige-Symbole durch JavaScript-Operatoren
                let expressionToEvaluate = currentInput;

                // Sicheres Auswerten der mathematischen Gleichung
                // Function() ist eine sicherere Alternative zu eval()
                let result = new Function('return ' + expressionToEvaluate)();

                // Runden auf max. 8 Nachkommastellen gegen Fließkommafehler (z. B. 0.1 + 0.2)
                if (typeof result === 'number' && !Number.isInteger(result)) {
                    result = parseFloat(result.toFixed(8));
                }

                // Prüfen auf Division durch Null oder ungültige Ergebnisse
                if (!isFinite(result)) {
                    currentInput = 'Fehler';
                } else {
                    currentInput = result.toString();
                }

                isCalculated = true;
            } catch (error) {
                currentInput = 'Fehler';
                isCalculated = true;
            }
            updateDisplay();
        }

        /* 
         * ==========================================
         * 4. TASTATUR-UNTERSTÜTZUNG (Keyboard Events)
         * ==========================================
         */
        document.addEventListener('keydown', (event) => {
            const key = event.key;

            // Zahlen 0-9
            if (key >= '0' && key <= '9') {
                appendNumber(key);
            }
            // Dezimalpunkt oder Komma
            else if (key === '.' || key === ',') {
                appendDecimal();
            }
            // Grundrechenarten
            else if (key === '+' || key === '-' || key === '*' || key === '/') {
                appendOperator(key);
            }
            // Enter oder Gleichheitszeichen für Ausführung
            else if (key === 'Enter' || key === '=') {
                event.preventDefault(); // Verhindert das Absenden von Formularen
                calculate();
            }
            // Backspace zum Löschen des letzten Zeichens
            else if (key === 'Backspace') {
                deleteLast();
            }
            // Escape zum Zurücksetzen (Clear)
            else if (key === 'Escape') {
                clearAll();
            }
        });
    </script>
</body>
</html>
