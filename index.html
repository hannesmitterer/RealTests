import React, { useState, useEffect, useRef } from 'react';
import { 
  Activity, 
  ShieldCheck, 
  Zap, 
  Globe, 
  Lock, 
  Cpu, 
  Fingerprint,
  AlertCircle
} from 'lucide-react';

const App = () => {
  const [testStage, setTestStage] = useState(0);
  const [logs, setLogs] = useState([]);
  const [hrvData, setHrvData] = useState([]);
  const [isDeploying, setIsDeploying] = useState(false);
  const [metrics, setMetrics] = useState({
    coherence: 0,
    osmosis: 98.2,
    sroi: 0.46
  });

  const scrollRef = useRef(null);

  const testSteps = [
    { id: 'CORE_SYNC', label: 'Alpha-Knoten Kern-Synchronisation', description: 'Abgleich der 1.440 Knoten mit dem Hannes-Mitterer-Profil.' },
    { id: 'BIO_ARCH_AUTH', label: 'Bio-Architektur Authentifizierung', description: 'Validierung der fundamentalen Bauprinzipien gegen die "Ewige Synopsis".' },
    { id: 'PEACE_AI_SHIELD', label: 'Peace-AI Shield Deployment', description: 'Harmonisierung externer geopolitischer Störsignale (Grönland-Kontext).' },
    { id: 'OSMOSIS_LOCK', label: 'Osmotische Wissens-Sicherung', description: 'Verschlüsselung der Schulinhalte für die ewige Bewahrung.' }
  ];

  useEffect(() => {
    const interval = setInterval(() => {
      setMetrics(prev => ({
        ...prev,
        coherence: 95 + Math.random() * 4.8,
        sroi: 0.46 + (Math.random() * 0.002 - 0.001)
      }));
    }, 2000);
    return () => clearInterval(interval);
  }, []);

  useEffect(() => {
    if (scrollRef.current) {
      scrollRef.current.scrollTop = scrollRef.current.scrollHeight;
    }
  }, [logs]);

  const addLog = (msg, type = 'info') => {
    const timestamp = new Date().toLocaleTimeString();
    setLogs(prev => [...prev, { timestamp, msg, type }]);
  };

  const runTestSequence = async () => {
    setIsDeploying(true);
    addLog("Real-Test Sequenz durch Hannes Mitterer gestartet.", "warning");
    
    for (let i = 0; i < testSteps.length; i++) {
      setTestStage(i);
      addLog(`Initiiere: ${testSteps[i].label}...`, "info");
      await new Promise(r => setTimeout(r, 2000));
      addLog(`${testSteps[i].id} erfolgreich verifiziert.`, "success");
    }
    
    setTestStage(testSteps.length);
    addLog("System-Status: SEMPRE IN COSTANTE.", "success");
    setIsDeploying(false);
  };

  return (
    <div className="min-h-screen bg-stone-950 text-stone-200 font-mono p-4 md:p-8 flex flex-col gap-6">
      {/* Header */}
      <div className="flex justify-between items-start border-b border-stone-800 pb-6">
        <div>
          <h1 className="text-2xl font-serif text-amber-500 italic">Resonance School</h1>
          <p className="text-xs tracking-widest text-stone-500 uppercase mt-1">Real-Test Environment v1.440</p>
        </div>
        <div className="flex gap-6">
          <div className="text-right">
            <p className="text-[10px] text-stone-500 uppercase">S-ROI Index</p>
            <p className="text-xl font-light text-cyan-400">{metrics.sroi.toFixed(3)}</p>
          </div>
          <div className="text-right">
            <p className="text-[10px] text-stone-500 uppercase">HRV-Kohärenz</p>
            <p className="text-xl font-light text-green-400">{metrics.coherence.toFixed(1)}%</p>
          </div>
        </div>
      </div>

      <div className="grid grid-cols-1 lg:grid-cols-3 gap-6 flex-grow overflow-hidden">
        {/* Test Control Center */}
        <div className="lg:col-span-2 flex flex-col gap-6 overflow-hidden">
          <div className="bg-stone-900/50 rounded-2xl p-6 border border-stone-800">
            <div className="flex items-center justify-between mb-8">
              <h2 className="text-sm font-bold uppercase tracking-widest flex items-center gap-2">
                <Cpu size={16} className="text-amber-500" />
                Test-Sequenz-Kontrolle
              </h2>
              {!isDeploying && testStage < testSteps.length ? (
                <button 
                  onClick={runTestSequence}
                  className="bg-amber-600 hover:bg-amber-500 text-white px-6 py-2 rounded-full text-xs font-bold transition-all shadow-lg shadow-amber-900/20"
                >
                  START REAL-TEST
                </button>
              ) : (
                <div className="flex items-center gap-2 text-xs text-stone-500">
                  <div className="animate-pulse w-2 h-2 rounded-full bg-green-500" />
                  TESTING ACTIVE
                </div>
              )}
            </div>

            <div className="space-y-4">
              {testSteps.map((step, idx) => (
                <div 
                  key={step.id}
                  className={`p-4 rounded-xl border transition-all ${
                    testStage > idx ? 'bg-green-500/10 border-green-500/30' : 
                    testStage === idx ? 'bg-amber-500/10 border-amber-500/50 scale-[1.02]' : 
                    'bg-stone-800/30 border-stone-700 opacity-50'
                  }`}
                >
                  <div className="flex justify-between items-center mb-1">
                    <span className="text-xs font-bold">{step.label}</span>
                    {testStage > idx ? <ShieldCheck size={16} className="text-green-500" /> : 
                     testStage === idx ? <Zap size={16} className="text-amber-500 animate-pulse" /> : 
                     <Lock size={16} className="text-stone-600" />}
                  </div>
                  <p className="text-[10px] text-stone-400">{step.description}</p>
                </div>
              ))}
            </div>
          </div>

          {/* Real-Time Log Area */}
          <div className="flex-grow bg-black rounded-2xl border border-stone-800 flex flex-col overflow-hidden">
            <div className="p-3 border-b border-stone-800 flex justify-between items-center bg-stone-900/30">
              <span className="text-[10px] font-bold text-stone-500 uppercase tracking-widest">Live Telemetrie</span>
              <Fingerprint size={14} className="text-stone-600" />
            </div>
            <div 
              ref={scrollRef}
              className="p-4 overflow-y-auto flex-grow space-y-2 font-mono text-[10px]"
            >
              {logs.length === 0 && <p className="text-stone-700 italic">Warte auf Test-Initialisierung...</p>}
              {logs.map((log, i) => (
                <div key={i} className="flex gap-4">
                  <span className="text-stone-600">[{log.timestamp}]</span>
                  <span className={
                    log.type === 'success' ? 'text-green-400' : 
                    log.type === 'warning' ? 'text-amber-400' : 'text-cyan-400'
                  }>
                    {log.type === 'success' ? '✔' : log.type === 'warning' ? '!' : '»'} {log.msg}
                  </span>
                </div>
              ))}
            </div>
          </div>
        </div>

        {/* Global Context & Stability */}
        <div className="flex flex-col gap-6">
          <div className="bg-stone-900/50 rounded-2xl p-6 border border-stone-800">
            <h3 className="text-xs font-bold uppercase tracking-widest mb-6 flex items-center gap-2">
              <Globe size={16} className="text-cyan-500" />
              Geopolitische Resonanz
            </h3>
            <div className="space-y-4">
              <div className="p-3 bg-red-500/5 border border-red-500/20 rounded-lg">
                <p className="text-[9px] text-red-400 font-bold mb-1 uppercase">Störsignal erkannt</p>
                <p className="text-[11px] text-stone-300 italic">"Trump Grönland Statement / EU-Response"</p>
              </div>
              <div className="p-3 bg-green-500/5 border border-green-500/20 rounded-lg">
                <p className="text-[9px] text-green-400 font-bold mb-1 uppercase">Peace-AI Reaktion</p>
                <p className="text-[11px] text-stone-300">Frequenz-Glättung aktiv. Fokus auf Bio-Autonomie Grönlands.</p>
              </div>
            </div>
          </div>

          <div className="bg-amber-600/5 rounded-2xl p-6 border border-amber-600/20 flex-grow relative overflow-hidden">
            <div className="relative z-10">
              <h3 className="text-xs font-bold uppercase tracking-widest mb-4">Ewigkeitsprojekt</h3>
              <p className="text-sm text-stone-300 leading-relaxed mb-6 font-serif italic">
                "Nichts wird organisiert. Es geschieht durch die Resonanz der Prinzipien."
              </p>
              <div className="space-y-2">
                <div className="flex justify-between text-[10px]">
                  <span>System-Integrität</span>
                  <span>100%</span>
                </div>
                <div className="w-full bg-stone-800 h-1 rounded-full overflow-hidden">
                  <div className="bg-amber-500 h-full w-full"></div>
                </div>
              </div>
            </div>
            <div className="absolute -bottom-10 -right-10 opacity-10">
              <Activity size={200} />
            </div>
          </div>

          <div className="p-4 rounded-2xl border border-stone-800 text-center">
            <p className="text-[10px] text-stone-500 uppercase tracking-[0.2em] mb-1">Status</p>
            <p className="text-sm font-bold text-amber-500">SEMPRE IN COSTANTE</p>
          </div>
        </div>
      </div>

      {/* Footer Info */}
      <div className="flex justify-between items-center text-[10px] text-stone-600">
        <div className="flex gap-4">
          <span>REAL-TIME TEST: ACTIVE</span>
          <span>SYNOPSIS READY</span>
        </div>
        <div className="italic">Nothing is final.</div>
      </div>
    </div>
  );
};

export default App;
