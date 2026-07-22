<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nautilus</title>
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
    <style>
        body {
            background-color: #0d0e12;
        }
        .node-card {
            background-color: #1e222b;
            border: 1px solid #2d3446;
        }
        /* Animazione dei puntini in movimento */
        .flow-line {
            stroke-dasharray: 6;
            animation: dash 0.8s linear infinite;
        }
        @keyframes dash {
            to { stroke-dashoffset: -12; }
        }
    </style>
</head>
<body class="text-gray-100 min-h-screen p-4 md:p-8 font-sans flex flex-col justify-center items-center">

    <div class="w-full max-w-4xl bg-[#11141c] p-8 rounded-3xl shadow-2xl border border-[#1f2535]">
        
        <div class="relative w-full overflow-x-auto pb-6 select-none">
            <div class="min-w-[800px] grid grid-cols-5 gap-y-12 items-center relative py-4">
                
                <svg class="absolute inset-0 w-full h-full pointer-events-none" style="z-index: 0;">
                    <path id="line-pendolo-1" d="M 120 48 L 200 48" stroke="#3f485f" stroke-width="2" />
                    <path id="line-pendolo-2" d="M 300 48 L 380 48" stroke="#3f485f" stroke-width="2" />
                    <path id="line-pendolo-3" d="M 480 48 L 560 48" stroke="#3f485f" stroke-width="2" />
                    <path id="line-tp1-bat" d="M 620 48 L 680 48 L 680 110 L 720 110" stroke="#3f485f" stroke-width="2" />

                    <path id="line-solare-1" d="M 120 172 L 200 172" stroke="#3f485f" stroke-width="2" />
                    <path id="line-solare-2" d="M 300 172 L 560 172" stroke="#3f485f" stroke-width="2" />
                    <path id="line-tp2-bat" d="M 620 172 L 680 172 L 680 110 L 720 110" stroke="#3f485f" stroke-width="2" />
                </svg>

                <div class="node-card z-10 w-28 h-20 rounded-xl flex flex-col items-center justify-center text-center px-2">
                    <span class="text-[10px] font-bold tracking-wider text-gray-400 uppercase">Gen. AC</span>
                    <span id="node_v_ac" class="text-sm font-bold mt-1 text-white">8.0V</span>
                </div>
                
                <div class="node-card z-10 w-28 h-20 rounded-xl flex flex-col items-center justify-center text-center px-2 relative">
                    <span class="text-[10px] font-bold tracking-wider text-gray-400 uppercase">Ponte Schottky</span>
                    <span id="node_v_rect" class="text-xs font-semibold mt-1 text-emerald-400">V_rect: 5.1V</span>
                    <div class="absolute -right-[13px] w-2 h-2 bg-blue-500 rounded-full top-[36px]"></div>
                </div>

                <div class="node-card z-10 w-28 h-20 rounded-xl flex flex-col items-center justify-center text-center px-2">
                    <span class="text-[10px] font-bold tracking-wider text-gray-400 uppercase">Buck-Boost</span>
                    <span id="node_v_bb" class="text-xs font-semibold mt-1 text-gray-300">OUT: 5.0V</span>
                </div>

                <div id="card_tp1" class="z-10 w-28 h-20 rounded-xl flex flex-col items-center justify-center text-center px-2 border transition-all duration-300 bg-sky-600/90 border-sky-400">
                    <span class="text-[10px] font-bold tracking-wider text-sky-100 uppercase">TP4056 (1)</span>
                    <span id="node_i_tp1" class="text-xs font-bold mt-1 text-white">1.0A</span>
                    <div class="absolute top-[64px] flex flex-col items-center">
                        <span id="flow_i_tp1" class="text-[10px] font-bold text-white bg-[#11141c] px-1 rounded">1.0A</span>
                        <div class="w-1.5 h-1.5 bg-blue-400 rounded-full mt-2"></div>
                    </div>
                </div>

                <div class="row-span-2 justify-self-end z-10 w-32 h-20 bg-purple-900/40 border border-purple-500/50 rounded-xl flex flex-col items-center justify-center text-center px-2 shadow-[0_0_15px_rgba(147,51,234,0.15)]">
                    <span class="text-[10px] font-bold tracking-wider text-purple-300 uppercase">3x 14500</span>
                    <span id="node_v_bat" class="text-sm font-black mt-1 text-purple-200">3.70V</span>
                </div>

                <div class="node-card z-10 w-28 h-20 rounded-xl flex flex-col items-center justify-center text-center px-2">
                    <span class="text-[10px] font-bold tracking-wider text-gray-400 uppercase">Pannello</span>
                    <span id="node_v_panel" class="text-sm font-bold mt-1 text-white">4.3V</span>
                </div>

                <div class="node-card z-10 w-28 h-20 rounded-xl flex flex-col items-center justify-center text-center px-2">
                    <span class="text-[10px] font-bold tracking-wider text-gray-400 uppercase">Protezione</span>
                    <span class="text-xs font-semibold mt-1 text-emerald-400">Diodo Schottky</span>
                </div>

                <div class="w-28 h-20 invisible"></div>

                <div id="card_tp2" class="z-10 w-28 h-24 rounded-xl flex flex-col items-center justify-center text-center px-2 border transition-all duration-300 bg-[#1e222b] border-[#2d3446]">
                    <span class="text-[10px] font-bold tracking-wider text-gray-400 uppercase">TP4056 (2)</span>
                    <span id="node_v_in2" class="text-[11px] font-semibold mt-0.5 text-gray-300">V_in2: 4.0V</span>
                    <span id="node_uvlo_status" class="text-[9px] font-black tracking-tighter text-red-400 mt-1 bg-red-950/80 px-1.5 py-0.5 rounded border border-red-800/40">UVLO BLOCCO</span>
                    <div class="absolute top-[142px] flex flex-col items-center">
                        <span id="flow_i_tp2" class="text-[10px] font-bold text-red-400 bg-[#11141c] px-1 rounded">0.0A</span>
                    </div>
                </div>

            </div>
        </div>

        <div class="flex flex-wrap gap-4 justify-center text-xs font-medium text-gray-400 mb-6 border-b border-gray-800 pb-4">
            <span class="flex items-center gap-1.5"><span class="w-2 h-2 rounded-full bg-blue-500"></span> Ramo Pendolo (AC)</span>
            <span class="flex items-center gap-1.5"><span class="w-2 h-2 rounded-full bg-emerald-500"></span> Ramo Solare (DC)</span>
            <span class="flex items-center gap-1.5"><span class="w-2 h-2 rounded-full bg-purple-500"></span> Batteria Litio</span>
        </div>

        <div class="grid grid-cols-2 gap-8 text-center my-6">
            <div>
                <span class="block text-xs font-bold tracking-wider text-gray-500 uppercase mb-1">Corrente Totale</span>
                <span id="summary_current" class="text-2xl font-black text-white tracking-tight">1.0 A</span>
            </div>
            <div>
                <span class="block text-xs font-bold tracking-wider text-gray-500 uppercase mb-1">Stato Sistema</span>
                <span id="summary_status" class="text-base font-mono font-bold text-cyan-400 mt-1 block">Ricarica (Solo Pendolo)</span>
            </div>
        </div>

        <hr class="border-gray-800 my-6">

        <div class="grid grid-cols-1 md:grid-cols-3 gap-x-8 gap-y-5">
            
            <div class="flex items-center justify-between gap-4">
                <label class="w-32 text-xs font-bold text-gray-400 uppercase tracking-wider">Pendolo AC (V)</label>
                <div class="flex-1 flex items-center gap-3">
                    <input type="range" id="input_v_ac" min="0" max="12" step="0.5" value="8" class="w-full h-1 bg-gray-800 rounded-lg appearance-none cursor-pointer accent-blue-500">
                    <span id="lbl_v_ac" class="w-12 text-center py-1 bg-[#1a1f2c] rounded-md border border-gray-800 text-sm font-semibold text-gray-200">8</span>
                </div>
            </div>

            <div class="flex items-center justify-between gap-4">
                <label class="w-32 text-xs font-bold text-gray-400 uppercase tracking-wider">Pannello DC (V)</label>
                <div class="flex-1 flex items-center gap-3">
                    <input type="range" id="input_v_panel" min="3.5" max="6.5" step="0.1" value="4.3" class="w-full h-1 bg-gray-800 rounded-lg appearance-none cursor-pointer accent-emerald-500">
                    <span id="lbl_v_panel" class="w-12 text-center py-1 bg-[#1a1f2c] rounded-md border border-gray-800 text-sm font-semibold text-gray-200">4,3</span>
                </div>
            </div>

            <div class="flex items-center justify-between gap-4">
                <label class="w-32 text-xs font-bold text-gray-400 uppercase tracking-wider">Stato Carica (V)</label>
                <div class="flex-1 flex items-center gap-3">
                    <input type="range" id="input_v_bat" min="3.0" max="4.2" step="0.05" value="3.7" class="w-full h-1 bg-gray-800 rounded-lg appearance-none cursor-pointer accent-purple-500">
                    <span id="lbl_v_bat" class="w-12 text-center py-1 bg-[#1a1f2c] rounded-md border border-gray-800 text-sm font-semibold text-gray-200">3,7</span>
                </div>
            </div>

        </div>

    </div>

    <script>
        const inVac = document.getElementById('input_v_ac');
        const inVpanel = document.getElementById('input_v_panel');
        const inVbat = document.getElementById('input_v_bat');

        // Configurazione Cadute di Tensione Diodi Schottky
        const drop_diode_schottky = 0.3;
        const drop_bridge_schottky = 0.6; // 2x diodi Schottky in serie sul ponte raddrizzatore

        function formatComma(val, decimals=1) {
            return val.toFixed(decimals).replace('.', ',');
        }

        function setLineState(id, isActive, activeColor) {
            const line = document.getElementById(id);
            if (isActive) {
                line.setAttribute('stroke', activeColor);
                line.classList.add('flow-line'); 
            } else {
                line.setAttribute('stroke', '#3f485f');
                line.classList.remove('flow-line'); 
            }
        }

        function runSim() {
            const v_ac = parseFloat(inVac.value);
            const v_panel = parseFloat(inVpanel.value);
            const v_bat = parseFloat(inVbat.value);

            document.getElementById('lbl_v_ac').innerText = formatComma(v_ac, 1);
            document.getElementById('lbl_v_panel').innerText = formatComma(v_panel, 1);
            document.getElementById('lbl_v_bat').innerText = formatComma(v_bat, 1);

            document.getElementById('node_v_ac').innerText = v_ac.toFixed(1) + "V";
            document.getElementById('node_v_panel').innerText = v_panel.toFixed(1) + "V";
            document.getElementById('node_v_bat').innerText = v_bat.toFixed(2) + "V";

            
            const v_rect = Math.max(0, (v_ac * 0.707) - drop_bridge_schottky);
            document.getElementById('node_v_rect').innerText = `V_rect: ${v_rect.toFixed(1)}V`;
            
            let v_bb = 0.0;
            let i_tp1 = 0.0;
            if (v_rect >= 2.5) {
                v_bb = 5.0;
                document.getElementById('node_v_bb').innerText = "OUT: 5.0V";
                if (v_bat < 4.2) i_tp1 = 1.0;
            } else {
                document.getElementById('node_v_bb').innerText = v_rect > 0 ? "LOW (<2.5)" : "OUT: 0.0V";
            }

            const cardTp1 = document.getElementById('card_tp1');
            if (i_tp1 > 0) {
                cardTp1.className = "z-10 w-28 h-20 rounded-xl flex flex-col items-center justify-center text-center px-2 border transition-all duration-300 bg-sky-600/90 border-sky-400 text-white";
                document.getElementById('node_i_tp1').innerText = "1.0A";
                document.getElementById('flow_i_tp1').innerText = "1.0A";
                document.getElementById('flow_i_tp1').className = "text-[10px] font-bold text-white bg-[#11141c] px-1 rounded";
            } else {
                cardTp1.className = "z-10 w-28 h-20 rounded-xl flex flex-col items-center justify-center text-center px-2 border transition-all duration-300 bg-[#1e222b] border-[#2d3446] text-gray-400";
                document.getElementById('node_i_tp1').innerText = "0.0A";
                document.getElementById('flow_i_tp1').innerText = "0.0A";
                document.getElementById('flow_i_tp1').className = "text-[10px] font-bold text-gray-500 bg-[#11141c] px-1 rounded";
            }

            
            const v_in2 = Math.max(0, v_panel - drop_diode_schottky);
            document.getElementById('node_v_in2').innerText = `V_in2: ${v_in2.toFixed(1)}V`;
            
            let i_tp2 = 0.0;
            const cardTp2 = document.getElementById('card_tp2');
            const uvloBadge = document.getElementById('node_uvlo_status');
            
            if (v_in2 < 4.5) {
                uvloBadge.classList.remove('hidden');
                cardTp2.className = "z-10 w-28 h-24 rounded-xl flex flex-col items-center justify-center text-center px-2 border transition-all duration-300 bg-[#1e222b] border-red-900/50";
                document.getElementById('flow_i_tp2').innerText = "0.0A UVLO BLOCCO";
                document.getElementById('flow_i_tp2').className = "text-[9px] font-bold text-red-400 bg-[#11141c] px-1 rounded text-center whitespace-nowrap mt-1";
            } else {
                uvloBadge.classList.add('hidden');
                if (v_bat < 4.2) {
                    i_tp2 = 1.0;
                    cardTp2.className = "z-10 w-28 h-24 rounded-xl flex flex-col items-center justify-center text-center px-2 border transition-all duration-300 bg-sky-600/90 border-sky-400 text-white";
                    document.getElementById('flow_i_tp2').innerText = "1.0A";
                    document.getElementById('flow_i_tp2').className = "text-[10px] font-bold text-white bg-[#11141c] px-1 rounded";
                } else {
                    cardTp2.className = "z-10 w-28 h-24 rounded-xl flex flex-col items-center justify-center text-center px-2 border transition-all duration-300 bg-[#1e222b] border-[#2d3446] text-gray-400";
                    document.getElementById('flow_i_tp2').innerText = "0.0A";
                    document.getElementById('flow_i_tp2').className = "text-[10px] font-bold text-gray-500 bg-[#11141c] px-1 rounded";
                }
            }

            
            let i_tot = i_tp1 + i_tp2;
            if (v_bat >= 4.2) {
                i_tot = 0;
                i_tp1 = 0;
                i_tp2 = 0;
            }

            document.getElementById('summary_current').innerText = i_tot.toFixed(1) + " A";
            
            let statusText = "Standby (Nessuna Fonte)";
            if (v_bat >= 4.2) {
                statusText = "Carica Completa (Isolato)";
            } else if (i_tp1 > 0 && i_tp2 > 0) {
                statusText = "Ricarica Combinata (Pendolo + Sole)";
            } else if (i_tp1 > 0) {
                statusText = "Ricarica (Solo Pendolo)";
            } else if (i_tp2 > 0) {
                statusText = "Ricarica (Solo Solare)";
            } else if (v_in2 < 4.5 && v_panel > 0 && i_tp1 === 0) {
                statusText = "Blocco Solare (Tensione Insufficiente)";
            }
            document.getElementById('summary_status').innerText = statusText;

            
            setLineState('line-pendolo-1', v_ac > 0, '#3b82f6');
            setLineState('line-pendolo-2', v_rect >= 2.5, '#3b82f6');
            setLineState('line-pendolo-3', v_bb > 0, '#3b82f6');
            setLineState('line-tp1-bat', i_tp1 > 0, '#3b82f6');
            
            setLineState('line-solare-1', v_panel > 0, '#10b981');
            setLineState('line-solare-2', v_in2 > 0, '#10b981');
            setLineState('line-tp2-bat', i_tp2 > 0, '#10b981');
        }

        inVac.addEventListener('input', runSim);
        inVpanel.addEventListener('input', runSim);
        inVbat.addEventListener('input', runSim);

        runSim();
    </script>
</body>
</html>
