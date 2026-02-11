import React, { useState, useEffect } from 'react';
import { 
  Video, 
  Users, 
  DollarSign, 
  TrendingUp, 
  ChevronRight, 
  Zap,
  Cpu,
  ShieldCheck,
  Building2,
  Share2,
  CheckCircle2
} from 'lucide-react';

const FLYWHEEL_DATA = [
  {
    id: 'execution',
    title: 'Core Engine: FB Corp Execution',
    subtitle: 'Real Projects, Real Data',
    icon: <Building2 className="w-6 h-6" />,
    color: 'text-blue-500',
    bg: 'bg-blue-500/10',
    border: 'border-blue-500/50',
    description: 'The foundation of the entire system. Without real execution, the rest is noise.',
    inputs: ['Multifamily Projects', 'ADUs', 'FL & AZ Expansion', 'Manufacturing via Build OS'],
    outputs: ['Revenue/Margins', 'Case Studies', 'Site Footage', 'Investor Proof'],
    tech: ['Drone Capture', 'Time-lapse Cameras', 'AI Note Capture (OAC)', 'Notion Milestones'],
  },
  {
    id: 'media',
    title: 'Media Engine',
    subtitle: 'Attention & Visibility',
    icon: <Video className="w-6 h-6" />,
    color: 'text-purple-500',
    bg: 'bg-purple-500/10',
    border: 'border-purple-500/50',
    description: 'Turning raw project material into long-form authority and discovery content.',
    inputs: ['Site Footage', 'War Stories', 'Cost Breakdowns', 'Lessons Learned'],
    outputs: ['Podcast Episodes', 'YouTube Deep Dives', 'Viral Reels/Shorts', 'UGC Clips'],
    tech: ['Batch Recording System', 'AI Transcription/Clips', 'Auto-scheduling (n8n)', 'AI Hook Testing'],
  },
  {
    id: 'skool',
    title: 'Skool: The Filter',
    subtitle: 'Community & Trust',
    icon: <Users className="w-6 h-6" />,
    color: 'text-orange-500',
    bg: 'bg-orange-500/10',
    border: 'border-orange-500/50',
    description: 'The pre-qualification layer. High-intent followers build loyalty before capital calls.',
    inputs: ['Behind-the-scenes content', 'Education', 'Direct Access'],
    outputs: ['Qualified Leads', 'Brand Advocates', 'Community Trust', 'Builder Network'],
    tech: ['Community Moderation', 'Exclusive Training Modules', 'Engagement Analytics'],
  },
  {
    id: 'capital',
    title: 'Reg A Capital Engine',
    subtitle: 'The Converter',
    icon: <DollarSign className="w-6 h-6" />,
    color: 'text-emerald-500',
    bg: 'bg-emerald-500/10',
    border: 'border-emerald-500/50',
    description: 'Converting warm audience trust into structured operating and acquisition capital.',
    inputs: ['Audience Trust', 'Deal Flow', 'Track Record'],
    outputs: ['Investor Commitments', 'Operating Capital', 'Land Acquisition'],
    tech: ['Investor Funnel Automation', 'AI Q&A Bot', 'CRM Tagging', 'Automated Webinars'],
  },
  {
    id: 'scale',
    title: 'Scale & Vertical Expansion',
    subtitle: 'The Accelerator',
    icon: <TrendingUp className="w-6 h-6" />,
    color: 'text-red-500',
    bg: 'bg-red-500/10',
    border: 'border-red-500/50',
    description: 'Capital enables bigger projects, which creates bigger content. The loop compounds.',
    inputs: ['Raised Capital', 'Vertical Integration', 'Institutional Interest'],
    outputs: ['Bigger Projects', 'Manufacturing ROI', 'Increased Valuation'],
    tech: ['Automated Cost Dashboards', 'ERP Integration', 'Scale Analytics'],
  },
];

const FlywheelSegment = ({ data, active, onClick, index, total }) => {
  const angle = (index / total) * 360;
  const rotateStyle = {
    transform: `rotate(${angle}deg) translateY(-140px) rotate(-${angle}deg)`,
  };

  return (
    <button
      onClick={() => onClick(data)}
      className={`absolute transition-all duration-500 ease-in-out p-4 rounded-full border-2 flex items-center justify-center hover:scale-110 shadow-lg ${
        active ? `${data.bg} ${data.border} scale-125 z-10` : 'bg-slate-900 border-slate-700 opacity-60'
      }`}
      style={rotateStyle}
    >
      <div className={active ? data.color : 'text-slate-400'}>
        {data.icon}
      </div>
    </button>
  );
};

export default function App() {
  const [activeSegment, setActiveSegment] = useState(FLYWHEEL_DATA[0]);
  const [isRotating, setIsRotating] = useState(true);
  const [copied, setCopied] = useState(false);

  useEffect(() => {
    if (!isRotating) return;
    const interval = setInterval(() => {
      setActiveSegment(prev => {
        const currentIndex = FLYWHEEL_DATA.findIndex(s => s.id === prev.id);
        return FLYWHEEL_DATA[(currentIndex + 1) % FLYWHEEL_DATA.length];
      });
    }, 5000);
    return () => clearInterval(interval);
  }, [isRotating]);

  const handleShare = () => {
    const dummyUrl = window.location.href;
    const textArea = document.createElement("textarea");
    textArea.value = dummyUrl;
    document.body.appendChild(textArea);
    textArea.select();
    document.execCommand('copy');
    document.body.removeChild(textArea);
    setCopied(true);
    setTimeout(() => setCopied(false), 2000);
  };

  return (
    <div className="min-h-screen bg-slate-950 text-slate-100 font-sans selection:bg-blue-500/30 p-4 md:p-8">
      <header className="max-w-7xl mx-auto mb-12 flex flex-col md:flex-row justify-between items-start md:items-center gap-6">
        <div>
          <h1 className="text-3xl font-bold tracking-tight text-white flex items-center gap-3">
            <Cpu className="w-8 h-8 text-blue-500" />
            FB CORP <span className="text-slate-500">2026</span> MASTER FLYWHEEL
          </h1>
          <p className="text-slate-400 mt-1">Integrated Growth Architecture & Operating System</p>
        </div>
        
        <div className="flex gap-3">
          <button 
            onClick={handleShare}
            className={`flex items-center gap-2 text-sm px-5 py-2.5 rounded-xl font-bold transition-all shadow-lg ${
              copied ? 'bg-emerald-600 text-white' : 'bg-white text-slate-950 hover:bg-slate-200'
            }`}
          >
            {copied ? <CheckCircle2 className="w-4 h-4" /> : <Share2 className="w-4 h-4" />}
            {copied ? 'Copied' : 'Share Dashboard'}
          </button>
          <button 
            onClick={() => setIsRotating(!isRotating)}
            className={`text-sm px-5 py-2.5 rounded-xl transition-all border font-bold ${
              isRotating ? 'bg-slate-900 border-slate-700 text-slate-400' : 'bg-blue-600/20 border-blue-500/50 text-blue-400'
            }`}
          >
            {isRotating ? 'Pause Loop' : 'Resume Loop'}
          </button>
        </div>
      </header>

      <div className="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
        <div className="lg:col-span-5 flex flex-col items-center justify-center py-12">
          <div className="relative w-80 h-80 flex items-center justify-center">
            <div className="absolute w-24 h-24 rounded-full bg-slate-900 border-4 border-slate-800 flex items-center justify-center z-20 shadow-[0_0_50px_rgba(59,130,246,0.2)]">
               <div className="text-center">
                  <span className="text-[10px] text-slate-500 block uppercase tracking-widest font-bold">Center</span>
                  <span className="text-sm font-black text-white">FB CORP</span>
               </div>
            </div>
            <div className="absolute w-64 h-64 rounded-full border border-slate-800/50 border-dashed animate-[spin_20s_linear_infinite]"></div>
            <div className="absolute w-40 h-40 rounded-full border border-blue-500/10 animate-[spin_15s_linear_infinite_reverse]"></div>
            {FLYWHEEL_DATA.map((segment, index) => (
              <FlywheelSegment
                key={segment.id}
                data={segment}
                index={index}
                total={FLYWHEEL_DATA.length}
                active={activeSegment.id === segment.id}
                onClick={(s) => {
                  setActiveSegment(s);
                  setIsRotating(false);
                }}
              />
            ))}
          </div>
          <div className="mt-16 w-full p-6 bg-slate-900/40 rounded-2xl border border-slate-800/50 backdrop-blur-sm">
             <div className="flex items-center gap-2 mb-4">
                <ShieldCheck className="w-4 h-4 text-emerald-500" />
                <span className="text-xs font-bold text-slate-400 uppercase tracking-widest">System Sequence</span>
             </div>
             <div className="flex flex-wrap items-center gap-2 text-xs font-bold text-slate-300">
               <span className="px-2 py-1 bg-slate-800 rounded">BUILD</span>
               <ChevronRight className="w-3 h-3 text-slate-600" />
               <span className="px-2 py-1 bg-slate-800 rounded">DOCUMENT</span>
               <ChevronRight className="w-3 h-3 text-slate-600" />
               <span className="px-2 py-1 bg-slate-800 rounded">PUBLISH</span>
               <ChevronRight className="w-3 h-3 text-slate-600" />
               <span className="px-2 py-1 bg-slate-800 rounded">CAPITAL</span>
               <ChevronRight className="w-3 h-3 text-slate-600" />
               <span className="px-2 py-1 bg-slate-800 rounded">SCALE</span>
             </div>
          </div>
        </div>

        <div className="lg:col-span-7">
          <div className={`p-8 md:p-10 rounded-[2.5rem] border transition-all duration-700 shadow-2xl min-h-[500px] flex flex-col ${activeSegment.bg} ${activeSegment.border}`}>
            <div className="flex items-start justify-between mb-10">
              <div>
                <div className={`mb-3 font-mono text-xs uppercase tracking-[0.3em] font-black ${activeSegment.color}`}>
                  Operational Layer
                </div>
                <h2 className="text-4xl md:text-5xl font-black text-white tracking-tight leading-none mb-3">
                  {activeSegment.title}
                </h2>
                <p className="text-xl text-slate-400 font-medium italic">
                  {activeSegment.subtitle}
                </p>
              </div>
              <div className={`p-5 rounded-3xl bg-black/40 border border-white/10 ${activeSegment.color}`}>
                {activeSegment.icon}
              </div>
            </div>

            <p className="text-slate-300 text-xl mb-12 leading-relaxed font-medium">
              {activeSegment.description}
            </p>

            <div className="grid md:grid-cols-2 gap-8 mt-auto">
              <div className="space-y-5">
                <h4 className="flex items-center gap-3 text-xs font-black text-slate-500 uppercase tracking-[0.2em]">
                  <div className="w-2 h-2 rounded-full bg-slate-500"></div>
                  Inputs / Raw Material
                </h4>
                <ul className="space-y-3">
                  {activeSegment.inputs.map((item, i) => (
                    <li key={i} className="flex items-center gap-3 text-base text-slate-100 font-semibold">
                      <div className={`w-1.5 h-1.5 rounded-full ${activeSegment.color.replace('text', 'bg')}`}></div>
                      {item}
                    </li>
                  ))}
                </ul>
              </div>

              <div className="space-y-5">
                <h4 className="flex items-center gap-3 text-xs font-black text-slate-500 uppercase tracking-[0.2em]">
                  <div className="w-2 h-2 rounded-full bg-blue-500"></div>
                  Tech & Optimization
                </h4>
                <div className="flex flex-wrap gap-2">
                  {activeSegment.tech.map((item, i) => (
                    <span key={i} className="flex items-center gap-2 text-xs font-bold text-slate-200 bg-black/40 px-3 py-2 rounded-lg border border-white/5">
                      <Zap className="w-3 h-3 text-yellow-500 shrink-0" />
                      {item}
                    </span>
                  ))}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  );
}
