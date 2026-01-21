<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Accelerator Calculator</title>
    <style>
        :root {
            --green-neon: #00ff00; --green-dark: #00cc00; --green-light: #90ff90;
            --green-medium: #00aa00; --green-bright: #39ff14; --green-top: #00ff88;
            --green-active: #00ff88; --green-glow: rgba(0, 255, 0, 0.3);
            --green-glow-light: rgba(0, 255, 0, 0.1); --green-top-glow: rgba(0, 255, 136, 0.4);
            --green-active-glow: rgba(0, 255, 136, 0.5); --black-primary: #000000;
            --white-primary: #ffffff; --moon-color: #b19cd9; --moon-glow: rgba(177, 156, 217, 0.3);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { 
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; 
            background: var(--black-primary); 
            color: var(--white-primary); 
            min-height: 100vh; 
            padding: 15px; 
            display: flex; 
            flex-direction: column; 
        }
        .container { max-width: 1400px; margin: 0 auto; width: 100%; flex: 1; }
        .header { 
            text-align: center; 
            padding: 15px 0; 
            margin-bottom: 15px; 
            border-bottom: 2px solid var(--green-glow); 
            position: relative; 
        }
        .main-title, .constructor-text {
            font-size: 2.8rem; 
            font-weight: 900; 
            text-transform: uppercase; 
            letter-spacing: 1px; 
            text-shadow: 0 0 10px var(--green-glow); 
            margin-bottom: 0; 
            margin-top: 0; 
        }
        .main-title { color: var(--green-neon); }
        .constructor-text { color: var(--green-bright); }
        
        .content-section { 
            background: rgba(10, 30, 10, 0.9); 
            border-radius: 15px; 
            padding: 25px; 
            margin-bottom: 20px; 
            border: 2px solid var(--green-glow); 
            width: 100%; 
            box-shadow: 0 0 15px var(--green-glow-light); 
        }
        .section-title { 
            color: var(--green-neon); 
            font-size: 1.5rem; 
            margin-bottom: 20px; 
            text-align: center; 
            text-shadow: 0 0 5px var(--green-glow); 
        }
        
        .reactions-container { display: flex; flex-wrap: wrap; justify-content: center; gap: 15px; width: 100%; }
        .reaction-btn { 
            flex: 1; 
            min-width: 200px; 
            max-width: 300px; 
            padding: 15px 10px; 
            background: rgba(0, 50, 0, 0.3); 
            border: 2px solid var(--green-glow); 
            border-radius: 12px; 
            color: var(--green-light); 
            cursor: pointer; 
            transition: all 0.3s ease; 
            text-align: center; 
            font-weight: 600; 
            font-size: 1.1rem; 
            display: flex; 
            flex-direction: column; 
            align-items: center; 
            gap: 8px; 
            height: 140px; 
            justify-content: center; 
        }
        .reaction-btn:hover { 
            background: rgba(0, 80, 0, 0.4); 
            border-color: var(--green-neon); 
            color: var(--green-neon); 
            transform: translateY(-3px); 
            box-shadow: 0 5px 15px var(--green-glow); 
        }
        .reaction-btn.active { 
            background: linear-gradient(135deg, var(--green-active), var(--green-dark)); 
            border-color: var(--green-active); 
            color: var(--black-primary); 
            font-weight: 700; 
            box-shadow: 0 0 25px var(--green-active-glow); 
        }
        .reaction-btn[data-reaction="moon_budding"]:hover { border-color: var(--moon-color); box-shadow: 0 5px 15px var(--moon-glow); }
        .reaction-btn[data-reaction="moon_budding"].active {
            background: linear-gradient(135deg, var(--moon-color), #8a74b8);
            border-color: var(--moon-color);
            box-shadow: 0 0 25px var(--moon-glow);
        }
        
        .reaction-icon { 
            font-size: 2rem; 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            gap: 0; 
            line-height: 1; 
            height: 35px; 
        }
        .reaction-icon.compact-emojis { 
            font-size: 0.6rem; 
            display: flex; 
            flex-wrap: wrap; 
            width: 2.5rem; 
            height: 2.5rem; 
            justify-content: center; 
            align-items: center; 
            gap: 0; 
        }
        .emoji-grid { 
            display: grid; 
            grid-template-columns: 1fr 1fr; 
            grid-template-rows: 1fr 1fr; 
            width: 100%; 
            height: 100%; 
            gap: 1px; 
            place-items: center; 
        }
        .emoji-cell { 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            width: 100%; 
            height: 100%; 
            font-size: 0.6rem; 
            line-height: 1; 
        }
        
        .reaction-content { 
            display: flex; 
            flex-direction: column; 
            align-items: center; 
            justify-content: center; 
            gap: 8px; 
            height: 100%; 
        }
        .reaction-top-row { 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            gap: 8px; 
            margin-bottom: 5px; 
        }
        .reaction-name { font-size: 1rem; font-weight: 600; margin-bottom: 5px; }
        .reaction-note { font-size: 0.75rem; font-weight: 500; color: var(--green-light); opacity: 0.8; margin-top: 3px; }
        .reaction-multiplier { 
            font-weight: 800; 
            color: var(--green-neon); 
            background: rgba(0, 100, 0, 0.3); 
            padding: 4px 10px; 
            border-radius: 15px; 
            font-size: 1rem; 
            border: 1px solid var(--green-glow); 
            margin-top: 5px; 
        }
        .reaction-btn.active .reaction-multiplier { color: var(--black-primary); background: rgba(255, 255, 255, 0.8); }
        .reaction-btn[data-reaction="moon_budding"] .reaction-multiplier {
            color: var(--moon-color);
            border-color: var(--moon-color);
            background: rgba(177, 156, 217, 0.2);
        }
        .reaction-btn[data-reaction="moon_budding"].active .reaction-multiplier {
            color: var(--black-primary);
            background: rgba(255, 255, 255, 0.9);
        }
        
        .params-toggle-container { 
            display: flex; 
            flex-wrap: wrap; 
            justify-content: center; 
            gap: 15px; 
            margin: 20px 0; 
            width: 100%; 
        }
        
        .param-toggle-btn {
            padding: 15px 30px;
            background: linear-gradient(135deg, var(--green-neon), var(--green-dark));
            border: 2px solid var(--green-neon);
            border-radius: 10px;
            color: var(--black-primary);
            font-size: 1.2rem;
            font-weight: 700;
            cursor: pointer;
            transition: all 0.3s ease;
            min-width: 250px;
            text-align: center;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            box-shadow: 0 0 15px var(--green-glow);
        }
        
        .dual-scale-toggle-container {
            display: flex;
            justify-content: center;
            margin: 25px 0 5px 0;
            width: 100%;
        }
        
        .dual-scale-btn {
            padding: 14px 28px;
            background: linear-gradient(135deg, var(--green-neon), var(--green-dark));
            border: 2px solid var(--green-neon);
            border-radius: 10px;
            color: var(--black-primary);
            font-size: 1.15rem;
            font-weight: 700;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 0 12px var(--green-glow);
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            min-width: 280px;
            height: 54px;
            position: relative;
            overflow: hidden;
            letter-spacing: 0.3px;
        }
        
        .dual-scale-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: 0.5s;
        }
        
        .dual-scale-btn:hover::before {
            left: 100%;
        }
        
        .dual-scale-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 25px var(--green-glow);
        }
        
        .dual-scale-btn.active {
            background: linear-gradient(135deg, var(--green-active), var(--green-medium));
            border-color: var(--green-active);
            box-shadow: 0 0 25px var(--green-active-glow);
        }
        
        .toggle-icon {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            font-size: 1.3rem;
            transition: transform 0.3s cubic-bezier(0.68, -0.55, 0.27, 1.55);
            width: 24px;
            height: 24px;
        }
        
        .param-toggle-btn .toggle-icon {
            font-size: 1.4rem;
        }
        
        .dual-scale-btn .toggle-icon {
            font-size: 1.2rem;
            width: 20px;
            height: 20px;
        }
        
        .param-toggle-btn.collapsed .toggle-icon,
        .dual-scale-btn.collapsed .toggle-icon {
            transform: rotate(0deg);
        }
        
        .param-toggle-btn.expanded .toggle-icon,
        .dual-scale-btn.active .toggle-icon {
            transform: rotate(180deg);
        }
        
        .param-toggle-btn:hover, .dual-scale-btn:hover { 
            transform: translateY(-3px); 
            box-shadow: 0 5px 25px var(--green-glow); 
        }
        
        .params-container, .bonus-container, .internal-bonus-container { 
            margin-top: 15px; 
            padding: 20px; 
            border-radius: 12px; 
            border: 2px solid var(--green-glow); 
            margin-bottom: 15px; 
            display: none;
            animation: fadeIn 0.3s ease;
        }
        .params-container.visible, .bonus-container.visible, .internal-bonus-container.visible { display: block; }
        .params-container { background: rgba(0, 30, 0, 0.4); }
        .bonus-container { background: rgba(0, 40, 0, 0.4); }
        .internal-bonus-container { background: rgba(0, 50, 0, 0.4); }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .params-grid, .bonus-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); 
            gap: 15px; 
        }
        .param-item, .bonus-input-container { display: flex; flex-direction: column; gap: 8px; }
        .param-label, .bonus-title, .params-title, .bonus-label { 
            color: var(--green-neon); 
            font-size: 1.2rem; 
            margin-bottom: 15px; 
            text-align: center; 
            font-weight: 600; 
            text-shadow: 0 0 5px var(--green-glow); 
        }
        .bonus-title, .params-title { font-size: 1.2rem; margin-bottom: 15px; }
        .param-label, .bonus-label { color: var(--green-light); font-size: 0.95rem; margin-bottom: 0; }
        
        .param-input, .bonus-input, .stat-input, .build-name-input { 
            padding: 12px 14px; 
            background: rgba(0, 0, 0, 0.4); 
            border: 2px solid var(--green-glow); 
            border-radius: 8px; 
            color: var(--green-light); 
            font-size: 1.1rem; 
            font-weight: 600; 
            width: 100%; 
            text-align: center; 
        }
        .stat-input, .build-name-input { text-align: left; }
        .skill-input { background: rgba(0, 50, 0, 0.3); }
        .param-input:focus, .bonus-input:focus, .stat-input:focus, .build-name-input:focus { 
            outline: none; 
            border-color: var(--green-neon); 
            box-shadow: 0 0 10px var(--green-glow); 
        }
        
        .builds-container { 
            display: grid; 
            grid-template-columns: repeat(auto-fill, minmax(500px, 1fr)); 
            gap: 20px; 
            margin-bottom: 25px; 
            width: 100%; 
        }
        .build-card { 
            background: rgba(10, 30, 10, 0.9); 
            border-radius: 15px; 
            padding: 25px; 
            border: 2px solid var(--green-glow); 
            width: 100%; 
            box-shadow: 0 0 10px var(--green-glow-light); 
        }
        .build-header { 
            display: flex; 
            justify-content: space-between; 
            align-items: center; 
            margin-bottom: 20px; 
            padding-bottom: 15px; 
            border-bottom: 2px solid var(--green-glow); 
        }
        .build-name-container { display: flex; align-items: center; gap: 15px; flex: 1; }
        .build-number { 
            width: 45px; height: 45px; 
            background: linear-gradient(135deg, var(--green-neon), var(--green-dark)); 
            border-radius: 50%; 
            display: flex; align-items: center; justify-content: center; 
            font-weight: bold; color: var(--black-primary); font-size: 1.3rem; 
            flex-shrink: 0; box-shadow: 0 0 10px var(--green-glow); 
        }
        .build-controls { display: flex; gap: 10px; }
        .delete-btn { 
            width: 50px; height: 50px; 
            border: none; border-radius: 8px; cursor: pointer; 
            display: flex; align-items: center; justify-content: center; 
            font-size: 1.8rem; 
            background: linear-gradient(135deg, var(--green-neon), var(--green-dark)); 
            color: var(--black-primary); transition: all 0.3s ease; 
            box-shadow: 0 0 10px var(--green-glow); 
        }
        .delete-btn:hover { 
            transform: translateY(-3px); box-shadow: 0 5px 15px var(--green-glow); 
            background: linear-gradient(135deg, #ff3333, #cc0000); 
        }
        
        .stats-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); 
            gap: 15px; 
            margin-bottom: 15px; 
        }
        .stat-item { display: flex; flex-direction: column; gap: 8px; }
        .stat-label { color: var(--green-light); font-weight: 600; font-size: 0.95rem; }
        
        .damage-results { 
            background: rgba(0, 30, 0, 0.4); 
            border-radius: 12px; 
            padding: 20px; 
            border: 2px solid var(--green-glow); 
        }
        .damage-title { 
            color: var(--green-neon); 
            font-size: 1.2rem; 
            margin-bottom: 15px; 
            text-align: center; 
            text-shadow: 0 0 5px var(--green-glow); 
        }
        .damage-values { display: grid; grid-template-columns: repeat(3, 1fr); gap: 15px; }
        .damage-value-item { 
            text-align: center; padding: 18px; 
            background: rgba(0, 20, 0, 0.3); border-radius: 8px; border: 1px solid var(--green-glow); 
        }
        .damage-label { color: var(--green-light); font-size: 0.9rem; margin-bottom: 8px; }
        .damage-value { 
            font-size: 1.5rem; font-weight: 700; color: var(--green-neon); 
            text-shadow: 0 0 5px var(--green-glow); 
        }
        .damage-value.error { color: #ff3333; font-size: 1.2rem; }
        .damage-crit-negative { color: #ff9999; }
        .damage-average { color: var(--green-neon); }
        .damage-crit-positive { color: #99ff99; }
        
        .controls-container { display: flex; justify-content: center; gap: 20px; margin: 30px 0; }
        .action-btn { 
            padding: 16px 30px; border: none; border-radius: 10px; 
            font-size: 1.2rem; font-weight: 600; cursor: pointer; 
            transition: all 0.3s ease; min-width: 250px; 
            display: flex; align-items: center; justify-content: center; gap: 10px; 
        }
        .add-build-btn { 
            background: linear-gradient(135deg, var(--green-neon), var(--green-dark)); 
            color: var(--black-primary); border: 2px solid var(--green-neon); 
            box-shadow: 0 0 15px var(--green-glow); 
        }
        .reset-btn { 
            background: linear-gradient(135deg, var(--green-dark), var(--green-medium)); 
            color: var(--white-primary); border: 2px solid var(--green-glow); 
            box-shadow: 0 0 10px var(--green-glow-light); 
        }
        .action-btn:hover { transform: translateY(-3px); box-shadow: 0 8px 25px var(--green-glow); }
        
        .comparison-section { overflow-x: auto; }
        .comparison-table { 
            width: 100%; border-collapse: collapse; margin-top: 15px; 
            font-size: 1rem; min-width: 700px; 
        }
        .comparison-table thead { display: table-header-group; }
        .comparison-table th { 
            background: rgba(0, 50, 0, 0.3); color: var(--green-neon); 
            padding: 14px 10px; text-align: center; border: 2px solid var(--green-glow); 
            white-space: nowrap; text-shadow: 0 0 5px var(--green-glow); font-size: 0.9rem; 
        }
        .comparison-table td { padding: 12px 10px; text-align: center; border: 1px solid rgba(0, 100, 0, 0.2); }
        .difference-cell { font-weight: 400; font-size: 0.95rem; }
        .difference-number, .difference-percent { font-weight: 300; }
        .difference-percent { opacity: 0.8; }
        .top-build { 
            color: var(--green-top); background: rgba(0, 80, 40, 0.3); 
            padding: 5px 15px; border-radius: 20px; font-weight: 700; 
            border: 1px solid var(--green-top); box-shadow: 0 0 8px var(--green-top-glow); 
        }
        .difference-negative { color: #ff6b6b; }
        .best-build { 
            background: linear-gradient(90deg, rgba(0, 60, 30, 0.5), rgba(0, 80, 40, 0.6)); 
            border-left: 4px solid var(--green-top); border-right: 4px solid var(--green-top); 
            box-shadow: 0 0 15px var(--green-top-glow); 
        }
        .comparison-table tbody tr:nth-child(odd) { background-color: rgba(10, 30, 10, 0.3); color: var(--green-light); }
        .comparison-table tbody tr:nth-child(even) { background-color: rgba(20, 40, 20, 0.3); color: var(--green-bright); }
        .comparison-table tbody tr.best-build:nth-child(odd) { 
            background: linear-gradient(90deg, rgba(0, 70, 35, 0.6), rgba(0, 90, 45, 0.7)); 
            color: var(--green-top); text-shadow: 0 0 5px var(--green-top-glow); 
        }
        .comparison-table tbody tr.best-build:nth-child(even) { 
            background: linear-gradient(90deg, rgba(0, 80, 40, 0.7), rgba(0, 100, 50, 0.8)); 
            color: var(--green-top); text-shadow: 0 0 5px var(--green-top-glow); 
        }
        .comparison-table tbody tr.best-build td { font-weight: 700; border-color: var(--green-top-glow); }
        
        .footer-container {
            text-align: center; padding: 20px; margin-top: 30px; 
            border-top: 1px solid var(--green-glow); background: rgba(0, 30, 0, 0.2); 
            border-radius: 10px; display: flex; flex-direction: column; gap: 15px;
        }
        .footer-buttons { display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; }
        .uid-button, .telegram-button {
            padding: 12px 25px; border-radius: 8px; font-size: 1.1rem; font-weight: 700; 
            cursor: pointer; transition: all 0.3s ease; box-shadow: 0 0 10px var(--green-glow); 
            min-width: 180px; display: flex; align-items: center; justify-content: center; text-decoration: none;
        }
        .uid-button {
            background: linear-gradient(135deg, var(--green-neon), var(--green-dark));
            border: 2px solid var(--green-neon); color: var(--black-primary);
        }
        .telegram-button {
            background: linear-gradient(135deg, #0088cc, #0055aa); border: 2px solid #0088cc;
            color: white; box-shadow: 0 0 10px rgba(0, 136, 204, 0.3);
        }
        .uid-button:hover, .telegram-button:hover { transform: translateY(-3px); box-shadow: 0 5px 20px var(--green-glow); }
        .telegram-button:hover { box-shadow: 0 5px 20px rgba(0, 136, 204, 0.5); }
        
        @media (max-width: 768px) { 
            .builds-container, .params-grid, .bonus-grid { grid-template-columns: 1fr; } 
            .main-title, .constructor-text { font-size: 2.2rem; }
            .reaction-icon { font-size: 1.8rem; }
            .reaction-icon.compact-emojis { font-size: 0.55rem; }
            .comparison-table { font-size: 0.9rem; min-width: 500px; }
            .param-toggle-btn { min-width: 200px; padding: 12px 20px; font-size: 1.1rem; }
            .dual-scale-btn { min-width: 240px; padding: 12px 20px; font-size: 1.05rem; height: 50px; }
            .footer-container { padding: 15px; }
            .footer-buttons { flex-direction: column; align-items: center; gap: 15px; }
            .uid-button, .telegram-button { width: 100%; max-width: 300px; min-width: auto; }
        }
        @media (max-width: 480px) { 
            .main-title, .constructor-text { font-size: 1.8rem; }
            .reaction-icon { font-size: 1.5rem; }
            .reaction-icon.compact-emojis { font-size: 0.5rem; }
            .comparison-table { font-size: 0.8rem; min-width: 400px; }
            .param-toggle-btn { width: 100%; min-width: auto; font-size: 1rem; padding: 10px 15px; }
            .dual-scale-btn { width: 100%; min-width: auto; padding: 10px 15px; font-size: 1rem; height: 48px; }
            .params-toggle-container { gap: 10px; }
            .controls-container { flex-direction: column; align-items: center; }
            .action-btn { width: 100%; min-width: auto; }
            .damage-values { grid-template-columns: 1fr; }
            .footer-container { padding: 10px; }
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="header">
            <h1 class="main-title">ACCELERATOR CALCULATOR</h1>
            <div class="constructor-text">CONSTRUCTOR</div>
        </header>
        
        <div class="content-section">
            <h2 class="section-title">ВЫБОР РЕАКЦИИ</h2>
            <div class="reactions-container" id="reactionsContainer"></div>
            
            <div class="params-toggle-container">
                <button class="param-toggle-btn collapsed" id="baseParamsToggle"><span class="toggle-icon">▼</span> БАЗОВЫЕ ПАРАМЕТРЫ</button>
                <button class="param-toggle-btn collapsed" id="externalBonusToggle"><span class="toggle-icon">▼</span> ВНЕШНИЕ БАФЫ</button>
                <button class="param-toggle-btn collapsed" id="internalBonusToggle"><span class="toggle-icon">▼</span> ВНУТРЕННИЕ БАФЫ</button>
            </div>
            
            <div class="params-container" id="baseParamsContainer">
                <div class="params-title">БАЗОВЫЕ ПАРАМЕТРЫ</div>
                <div class="params-grid" id="baseParamsGrid"></div>
            </div>
            
            <div class="bonus-container" id="externalBonusContainer">
                <div class="bonus-title">ВНЕШНИЕ БАФЫ</div>
                <div class="bonus-grid" id="externalBonusGrid"></div>
            </div>
            
            <div class="internal-bonus-container" id="internalBonusContainer">
                <div class="bonus-title">ВНУТРЕННИЕ БАФЫ</div>
                <div class="bonus-grid" id="internalBonusGrid"></div>
                <div class="dual-scale-toggle-container">
                    <button class="dual-scale-btn collapsed" id="dualScaleToggle"><span class="toggle-icon">▼</span> СДВОЕННЫЙ СКЕЙЛ</button>
                </div>
            </div>
        </div>
        
        <div class="builds-container" id="buildsContainer"></div>
        
        <div class="controls-container">
            <button class="action-btn add-build-btn" id="addBuildBtn"><span style="font-size: 1.4rem;">+</span> ДОБАВИТЬ СБОРКУ</button>
            <button class="action-btn reset-btn" id="resetBtn"><span style="font-size: 1.3rem;">↻</span> СБРОСИТЬ ВСЕ</button>
        </div>
        
        <div class="content-section comparison-section">
            <h2 class="section-title">СРАВНЕНИЕ СБОРОК</h2>
            <table class="comparison-table">
                <thead><tr><th>Сборка</th><th>Отставание</th><th>-Крит</th><th>Средний</th><th>+Крит</th></tr></thead>
                <tbody id="comparisonBody"></tbody>
            </table>
        </div>
        
        <div class="footer-container">
            <div class="footer-buttons">
                <button class="uid-button" id="uidButton">UID 728765572</button>
                <a href="https://t.me/AcCalConsBot" target="_blank" class="telegram-button">Telegram</a>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => new AcceleratorCalculator().init());
        
        class AcceleratorCalculator {
            constructor() {
                this.CONFIG = {
                    MAX_BUILDS: 10,
                    DEFAULT_VALUES: { skillMultiplier: 100, scale: 2000, critRate: 75, critDmg: 150, em: 150, affixBonus: 46.6 },
                    DUAL_SCALE_DEFAULT_VALUES: { skillMultiplier1: 50, skillMultiplier2: 50, scale1: 2000, scale2: 2000, critRate: 75, critDmg: 150, em: 150, affixBonus: 46.6 }
                };
                
                this.LEVEL_MULTIPLIERS = {
                    aggravate: { 1:20, 10:39, 20:93, 30:157, 40:238, 50:372, 60:567, 70:880, 80:1239, 90:1664, 95:1910, 100:2155 },
                    spread: { 1:22, 10:43, 20:101, 30:170, 40:259, 50:405, 60:616, 70:957, 80:1347, 90:1809, 95:2076, 100:2343 }
                };
                
                this.REACTIONS = {
                    no_reaction: { name: 'Без реакции', baseMultiplier: 1.0, type: 'standard', needsEM: false },
                    vaporize_reverse: { name: 'Обратные', baseMultiplier: 1.5, type: 'amplifying', needsEM: true },
                    vaporize_forward: { name: 'Пар/Таяние', baseMultiplier: 2.0, type: 'amplifying', needsEM: true },
                    aggravate: { name: 'Обострение', baseMultiplier: 1.15, type: 'catalyze', needsEM: true },
                    spread: { name: 'Разрастание', baseMultiplier: 1.25, type: 'catalyze', needsEM: true },
                    moon_budding: { name: 'Лунные реакции', baseMultiplier: 2.8, type: 'moon_budding', needsEM: true }
                };
                
                this.state = {
                    currentReaction: 'no_reaction',
                    builds: [],
                    maxBuildId: 0,
                    dualScaleMode: false,
                    globalCharLevel: 90,
                    globalEnemyLevel: 95,
                    globalEnemyRes: 10,
                    flatScaleBonus: 0,
                    emBonus: 0,
                    affixBonusBonus: 0,
                    specialMultiplier: 100,
                    flatDamageBonus: 0,
                    reactionBonus: 0,
                    defReduction: 0,
                    defIgnore: 0,
                    directMultiplier: 100
                };
                
                this.inputConfigs = {
                    base: [
                        { id: 'charLevelInput', label: 'Уровень персонажа', min: 1, max: 100, step: 1, value: 90, placeholder: '1-100' },
                        { id: 'enemyLevelInput', label: 'Уровень врага', min: 1, max: 150, step: 1, value: 95, placeholder: '1-150' },
                        { id: 'enemyResInput', label: 'Резист врага %', min: -100, max: 100, step: 1, value: 10, placeholder: '-100 до 100' }
                    ],
                    external: [
                        { id: 'flatScaleInput', label: '+ Скейл', min: 0, max: 10000, step: 10, value: 0, placeholder: '0-10000' },
                        { id: 'emBonusInput', label: '+ МС', min: 0, max: 2000, step: 10, value: 0, placeholder: '0-2000' },
                        { id: 'affixBonusInput', label: '+ Бонус урона %', min: 0, max: 200, step: 0.1, value: 0, placeholder: '0-200' }
                    ],
                    internal: [
                        { id: 'specialMultiplierInput', label: 'Специальный множитель %', min: 0, max: 500, step: 0.1, value: 100, placeholder: '0-500' },
                        { id: 'flatDamageInput', label: '+ Добавочный урон', min: 0, max: 10000, step: 10, value: 0, placeholder: '0-10000' },
                        { id: 'reactionBonusInput', label: 'Бонус реакции %', min: 0, max: 200, step: 0.1, value: 0, placeholder: '0-200' },
                        { id: 'defReductionInput', label: 'Снижение защиты %', min: 0, max: 90, step: 1, value: 0, placeholder: '0-90' },
                        { id: 'defIgnoreInput', label: 'Игнорирование защиты %', min: 0, max: 100, step: 1, value: 0, placeholder: '0-100' },
                        { id: 'directMultiplierInput', label: 'Прямой множитель %', min: 0, max: 500, step: 0.1, value: 100, placeholder: '0-500' }
                    ]
                };
                
                this.reactionIcons = {
                    no_reaction: '<div class="reaction-icon">🚫</div>',
                    vaporize_reverse: '<div class="reaction-icon compact-emojis"><div class="emoji-grid"><div class="emoji-cell">🔥</div><div class="emoji-cell">💧</div><div class="emoji-cell">❄️</div><div class="emoji-cell">🔥</div></div></div>',
                    vaporize_forward: '<div class="reaction-icon compact-emojis"><div class="emoji-grid"><div class="emoji-cell">💧</div><div class="emoji-cell">🔥</div><div class="emoji-cell">🔥</div><div class="emoji-cell">❄️</div></div></div>',
                    aggravate: '<div class="reaction-icon aggravate"><div class="aggravate-main">⚡️</div><div class="aggravate-small"><div>⚡️</div><div>🌱</div></div></div>',
                    spread: '<div class="reaction-icon spread"><div class="spread-main">🌱</div><div class="spread-small"><div>⚡️</div><div>🌱</div></div></div>',
                    moon_budding: '<div class="reaction-icon moon-budding">🌙</div>'
                };
            }
            
            init() {
                this.createReactionButtons();
                this.createInputFields();
                this.setupEventListeners();
                this.setupToggleButtons();
                this.addBuild();
            }
            
            parseNumber(value, defaultValue = 0) {
                if (value == null || value === '') return defaultValue;
                const num = parseFloat(value);
                return isNaN(num) ? defaultValue : num;
            }
            
            clamp(value, min, max) {
                return Math.min(max, Math.max(min, value));
            }
            
            formatNumber(num, exact = false) {
                if (num == null || isNaN(num)) return "0";
                const rounded = Math.round(num);
                if (exact) return rounded.toLocaleString('ru-RU');
                if (rounded >= 1e6) return (rounded / 1e6).toFixed(2) + 'M';
                if (rounded >= 1e3) return (rounded / 1e3).toFixed(1) + 'K';
                return rounded.toLocaleString('ru-RU');
            }
            
            createReactionButtons() {
                const container = document.getElementById('reactionsContainer');
                const reactions = [
                    { id: 'no_reaction', name: 'Без реакции', multiplier: 'х1.0' },
                    { id: 'vaporize_reverse', name: 'Обратные', multiplier: 'х1.5' },
                    { id: 'vaporize_forward', name: 'Пар/Таяние', multiplier: 'х2.0' },
                    { id: 'aggravate', name: 'Обострение', multiplier: 'х1.15' },
                    { id: 'spread', name: 'Разрастание', multiplier: 'х1.25' },
                    { id: 'moon_budding', name: 'Лунные реакции', multiplier: 'х2.8', note: '(только для сравнения сборок)' }
                ];
                
                reactions.forEach(reaction => {
                    const btn = document.createElement('button');
                    btn.className = `reaction-btn ${reaction.id === 'no_reaction' ? 'active' : ''}`;
                    btn.dataset.reaction = reaction.id;
                    btn.innerHTML = `
                        <div class="reaction-content">
                            <div class="reaction-name">${reaction.name}</div>
                            <div class="reaction-top-row">
                                ${this.reactionIcons[reaction.id]}
                                <div class="reaction-multiplier">${reaction.multiplier}</div>
                            </div>
                            ${reaction.note ? `<div class="reaction-note">${reaction.note}</div>` : ''}
                        </div>
                    `;
                    container.appendChild(btn);
                });
            }
            
            createInputFields() {
                this.createInputGroup('baseParamsGrid', this.inputConfigs.base);
                this.createInputGroup('externalBonusGrid', this.inputConfigs.external);
                this.createInputGroup('internalBonusGrid', this.inputConfigs.internal);
            }
            
            createInputGroup(containerId, configs) {
                const container = document.getElementById(containerId);
                configs.forEach(config => {
                    const item = document.createElement('div');
                    item.className = containerId.includes('base') ? 'param-item' : 'bonus-input-container';
                    item.innerHTML = `
                        <div class="${containerId.includes('base') ? 'param-label' : 'bonus-label'}">${config.label}</div>
                        <input type="number" class="${containerId.includes('base') ? 'param-input' : 'bonus-input'}" 
                               id="${config.id}" min="${config.min}" max="${config.max}" step="${config.step}" 
                               value="${config.value}" placeholder="${config.placeholder}">
                    `;
                    container.appendChild(item);
                });
            }
            
            setupEventListeners() {
                document.querySelectorAll('.reaction-btn').forEach(btn => {
                    btn.addEventListener('click', () => this.selectReaction(btn.dataset.reaction));
                });
                
                document.getElementById('addBuildBtn').addEventListener('click', () => this.addBuild());
                document.getElementById('resetBtn').addEventListener('click', () => this.resetAll());
                document.getElementById('dualScaleToggle').addEventListener('click', () => this.toggleDualScale());
                
                this.inputConfigs.base.concat(this.inputConfigs.external, this.inputConfigs.internal)
                    .forEach(config => this.setupGlobalInput(config.id));
                
                document.getElementById('uidButton').addEventListener('click', this.copyUID);
            }
            
            setupGlobalInput(inputId) {
                const element = document.getElementById(inputId);
                if (!element) return;
                
                element.addEventListener('input', (e) => {
                    const value = e.target.value;
                    
                    if (value === '') {
                        this.state[this.getStateKey(inputId)] = 0;
                        element.value = 0;
                        this.updateAllBuilds();
                        return;
                    }
                    
                    const numValue = this.parseNumber(value, 0);
                    this.state[this.getStateKey(inputId)] = numValue;
                    element.value = numValue;
                    this.updateAllBuilds();
                });
                
                element.addEventListener('blur', (e) => {
                    if (e.target.value === '') {
                        element.value = 0;
                        this.state[this.getStateKey(inputId)] = 0;
                        this.updateAllBuilds();
                    }
                });
            }
            
            getStateKey(inputId) {
                const map = {
                    charLevelInput: 'globalCharLevel',
                    enemyLevelInput: 'globalEnemyLevel',
                    enemyResInput: 'globalEnemyRes',
                    flatScaleInput: 'flatScaleBonus',
                    emBonusInput: 'emBonus',
                    affixBonusInput: 'affixBonusBonus',
                    specialMultiplierInput: 'specialMultiplier',
                    flatDamageInput: 'flatDamageBonus',
                    reactionBonusInput: 'reactionBonus',
                    defReductionInput: 'defReduction',
                    defIgnoreInput: 'defIgnore',
                    directMultiplierInput: 'directMultiplier'
                };
                return map[inputId] || inputId;
            }
            
            setupToggleButtons() {
                const toggles = [
                    ['baseParamsToggle', 'baseParamsContainer'],
                    ['externalBonusToggle', 'externalBonusContainer'],
                    ['internalBonusToggle', 'internalBonusContainer']
                ];
                
                toggles.forEach(([toggleId, containerId]) => {
                    const toggle = document.getElementById(toggleId);
                    const container = document.getElementById(containerId);
                    
                    toggle.addEventListener('click', () => {
                        const wasCollapsed = toggle.classList.contains('collapsed');
                        
                        toggles.forEach(([otherToggleId, otherContainerId]) => {
                            if (otherToggleId !== toggleId) {
                                const otherToggle = document.getElementById(otherToggleId);
                                const otherContainer = document.getElementById(otherContainerId);
                                otherContainer.classList.remove('visible');
                                otherToggle.classList.add('collapsed');
                                otherToggle.classList.remove('expanded');
                            }
                        });
                        
                        container.classList.toggle('visible');
                        
                        if (wasCollapsed) {
                            toggle.classList.remove('collapsed');
                            toggle.classList.add('expanded');
                        } else {
                            toggle.classList.remove('expanded');
                            toggle.classList.add('collapsed');
                        }
                    });
                    
                    container.classList.remove('visible');
                    toggle.classList.add('collapsed');
                    toggle.classList.remove('expanded');
                });
            }
            
            selectReaction(reaction) {
                this.state.currentReaction = reaction;
                document.querySelectorAll('.reaction-btn').forEach(btn => {
                    btn.classList.toggle('active', btn.dataset.reaction === reaction);
                });
                this.updateAllBuilds();
            }
            
            addBuild() {
                if (this.state.builds.length >= this.CONFIG.MAX_BUILDS) {
                    alert(`Максимум ${this.CONFIG.MAX_BUILDS} сборок!`);
                    return;
                }
                
                this.state.maxBuildId++;
                const buildId = this.state.maxBuildId;
                
                let values;
                if (this.state.builds.length > 0) {
                    const lastBuild = this.state.builds[this.state.builds.length - 1];
                    values = { ...lastBuild.values };
                } else {
                    values = this.state.dualScaleMode ? 
                        { ...this.CONFIG.DUAL_SCALE_DEFAULT_VALUES } : 
                        { ...this.CONFIG.DEFAULT_VALUES };
                }
                
                const build = {
                    id: buildId,
                    name: `Сборка ${buildId}`,
                    values: values,
                    damage: { min: 0, avg: 0, max: 0 },
                    difference: 0,
                    differencePercent: 0,
                    isTop: false
                };
                
                this.state.builds.push(build);
                this.createBuildCard(build);
                this.calculateBuildDamage(buildId);
            }
            
            createBuildCard(build) {
                const container = document.getElementById('buildsContainer');
                const card = document.createElement('div');
                card.className = 'build-card';
                card.id = `build-${build.id}`;
                
                if (this.state.dualScaleMode) {
                    card.innerHTML = this.getDualScaleBuildHTML(build);
                } else {
                    card.innerHTML = this.getSingleScaleBuildHTML(build);
                }
                
                container.appendChild(card);
                this.setupBuildCardListeners(build.id);
            }
            
            getSingleScaleBuildHTML(build) {
                return `
                    <div class="build-header">
                        <div class="build-name-container">
                            <div class="build-number">${build.id}</div>
                            <input type="text" class="build-name-input" value="${build.name}" data-build="${build.id}" maxlength="20">
                        </div>
                        <div class="build-controls">
                            <button class="delete-btn" data-build="${build.id}" title="Удалить сборку">❌</button>
                        </div>
                    </div>
                    <div class="stats-grid">
                        ${this.createStatInput(build.id, 'skillMultiplier', 'Множитель навыка %', build.values.skillMultiplier, 1, null, 1, true)}
                        ${this.createStatInput(build.id, 'scale', 'Скейл', build.values.scale, 0, null, 10)}
                        ${this.createStatInput(build.id, 'critRate', 'Крит Шанс %', build.values.critRate, 0, 100, 0.1)}
                        ${this.createStatInput(build.id, 'critDmg', 'Крит Урон %', build.values.critDmg, 0, null, 0.1)}
                        ${this.createStatInput(build.id, 'em', 'МС', build.values.em, 0, null, 1)}
                        ${this.createStatInput(build.id, 'affixBonus', 'Бонус урона %', build.values.affixBonus, 0, null, 0.1)}
                    </div>
                    <div class="damage-results">
                        <div class="damage-title" id="damageTitle-${build.id}">${this.REACTIONS[this.state.currentReaction].name.toUpperCase()}</div>
                        <div class="damage-values">
                            ${this.createDamageValue(build.id, 'min', '-КРИТ', 'damage-crit-negative')}
                            ${this.createDamageValue(build.id, 'avg', 'СРЕДНИЙ', 'damage-average')}
                            ${this.createDamageValue(build.id, 'max', '+КРИТ', 'damage-crit-positive')}
                        </div>
                    </div>
                `;
            }
            
            getDualScaleBuildHTML(build) {
                return `
                    <div class="build-header">
                        <div class="build-name-container">
                            <div class="build-number">${build.id}</div>
                            <input type="text" class="build-name-input" value="${build.name}" data-build="${build.id}" maxlength="20">
                        </div>
                        <div class="build-controls">
                            <button class="delete-btn" data-build="${build.id}" title="Удалить сборку">❌</button>
                        </div>
                    </div>
                    <div class="stats-grid">
                        ${this.createStatInput(build.id, 'skillMultiplier1', 'Множитель навыка №1 %', build.values.skillMultiplier1, 1, null, 1, true)}
                        ${this.createStatInput(build.id, 'skillMultiplier2', 'Множитель навыка №2 %', build.values.skillMultiplier2, 1, null, 1, true)}
                        ${this.createStatInput(build.id, 'scale1', 'Скейл №1', build.values.scale1, 0, null, 10)}
                        ${this.createStatInput(build.id, 'scale2', 'Скейл №2', build.values.scale2, 0, null, 10)}
                        ${this.createStatInput(build.id, 'critRate', 'Крит Шанс %', build.values.critRate, 0, 100, 0.1)}
                        ${this.createStatInput(build.id, 'critDmg', 'Крит Урон %', build.values.critDmg, 0, null, 0.1)}
                        ${this.createStatInput(build.id, 'em', 'МС', build.values.em, 0, null, 1)}
                        ${this.createStatInput(build.id, 'affixBonus', 'Бонус урона %', build.values.affixBonus, 0, null, 0.1)}
                    </div>
                    <div class="damage-results">
                        <div class="damage-title" id="damageTitle-${build.id}">${this.REACTIONS[this.state.currentReaction].name.toUpperCase()}</div>
                        <div class="damage-values">
                            ${this.createDamageValue(build.id, 'min', '-КРИТ', 'damage-crit-negative')}
                            ${this.createDamageValue(build.id, 'avg', 'СРЕДНИЙ', 'damage-average')}
                            ${this.createDamageValue(build.id, 'max', '+КРИТ', 'damage-crit-positive')}
                        </div>
                    </div>
                `;
            }
            
            createStatInput(buildId, type, label, value, min, max, step, isSkill = false) {
                return `
                    <div class="stat-item">
                        <div class="stat-label">${label}</div>
                        <input type="number" class="stat-input ${isSkill ? 'skill-input' : ''}" 
                               data-build="${buildId}" data-type="${type}" 
                               value="${value}" 
                               ${min !== null ? `min="${min}"` : ''} 
                               ${max !== null ? `max="${max}"` : ''} 
                               step="${step}">
                    </div>
                `;
            }
            
            createDamageValue(buildId, type, label, className) {
                return `
                    <div class="damage-value-item">
                        <div class="damage-label">${label}</div>
                        <div class="damage-value ${className}" id="${type}Damage-${buildId}">0</div>
                    </div>
                `;
            }
            
            getDefaultValue(type) {
                const defaults = {
                    skillMultiplier: 100, 
                    skillMultiplier1: 50, 
                    skillMultiplier2: 50,
                    scale: 2000, 
                    scale1: 2000, 
                    scale2: 2000,
                    critRate: 75, 
                    critDmg: 150, 
                    em: 150, 
                    affixBonus: 46.6
                };
                return defaults[type] || 0;
            }
            
            setupBuildCardListeners(buildId) {
                const card = document.getElementById(`build-${buildId}`);
                if (!card) return;
                
                card.querySelector('.build-name-input').addEventListener('input', (e) => {
                    const build = this.state.builds.find(b => b.id === buildId);
                    if (build) {
                        build.name = e.target.value;
                        this.updateComparisonTable();
                    }
                });
                
                card.querySelectorAll('.stat-input').forEach(input => {
                    const type = input.dataset.type;
                    const defaultValue = this.getDefaultValue(type);
                    
                    input.addEventListener('input', (e) => {
                        const value = e.target.value;
                        
                        if (value === '') {
                            input.value = 0;
                            const build = this.state.builds.find(b => b.id === buildId);
                            if (build) {
                                build.values[type] = 0;
                                this.calculateBuildDamage(buildId);
                            }
                            return;
                        }
                        
                        let numValue = this.parseNumber(value, defaultValue);
                        
                        if (type.includes('skillMultiplier') && numValue < 1) numValue = 1;
                        if (type === 'critRate') numValue = this.clamp(numValue, 0, 100);
                        if (type.includes('scale') || type === 'em' || type === 'affixBonus' || type === 'critDmg') {
                            if (numValue < 0) numValue = 0;
                        }
                        
                        input.value = numValue;
                        const build = this.state.builds.find(b => b.id === buildId);
                        if (build) {
                            build.values[type] = numValue;
                            this.calculateBuildDamage(buildId);
                        }
                    });
                    
                    input.addEventListener('blur', (e) => {
                        if (e.target.value === '') {
                            input.value = 0;
                            const build = this.state.builds.find(b => b.id === buildId);
                            if (build) {
                                build.values[type] = 0;
                                this.calculateBuildDamage(buildId);
                            }
                        }
                    });
                });
                
                card.querySelector('.delete-btn').addEventListener('click', () => {
                    if (this.state.builds.length <= 1) {
                        alert('Должна остаться хотя бы одна сборка!');
                        return;
                    }
                    this.removeBuild(buildId);
                });
            }
            
            removeBuild(buildId) {
                this.state.builds = this.state.builds.filter(b => b.id !== buildId);
                const card = document.getElementById(`build-${buildId}`);
                if (card) card.remove();
                this.updateComparisonTable();
            }
            
            calculateBuildDamage(buildId) {
                const build = this.state.builds.find(b => b.id === buildId);
                if (!build) return;
                
                try {
                    const damage = this.calculateDamage(build);
                    build.damage = damage;
                    this.updateBuildDisplay(buildId, damage);
                    this.updateComparisonTable();
                } catch (error) {
                    console.error(`Ошибка расчета для сборки ${buildId}:`, error);
                    this.showDamageError(buildId);
                }
            }
            
            calculateDamage(build) {
                const reaction = this.REACTIONS[this.state.currentReaction];
                const values = build.values;
                
                const totalAffixBonus = this.parseNumber(values.affixBonus, 46.6) + this.state.affixBonusBonus;
                const critRate = Math.min(1, this.parseNumber(values.critRate, 75) / 100);
                const critDmg = this.parseNumber(values.critDmg, 150) / 100;
                const critMultiplier = 1 + (critRate * critDmg);
                
                const defMultiplier = this.calculateDefMultiplier();
                const resMultiplier = this.calculateResMultiplier();
                const directMultiplierValue = this.state.directMultiplier / 100;
                const specialMultiplierValue = this.state.specialMultiplier / 100;
                const totalEM = this.parseNumber(values.em, 150) + this.state.emBonus;
                const reactionBonusValue = this.state.reactionBonus / 100;
                
                let baseDamage = 0;
                if (this.state.dualScaleMode) {
                    const skill1 = this.parseNumber(values.skillMultiplier1, 50) / 100;
                    const skill2 = this.parseNumber(values.skillMultiplier2, 50) / 100;
                    const scale1 = this.parseNumber(values.scale1, 2000) + this.state.flatScaleBonus;
                    const scale2 = this.parseNumber(values.scale2, 2000) + this.state.flatScaleBonus;
                    baseDamage = (skill1 * scale1) + (skill2 * scale2);
                } else {
                    const skill = this.parseNumber(values.skillMultiplier, 100) / 100;
                    const scale = this.parseNumber(values.scale, 2000) + this.state.flatScaleBonus;
                    baseDamage = skill * scale;
                }
                
                const damageWithSpecial = (baseDamage * specialMultiplierValue) + this.state.flatDamageBonus;
                const damageWithAffix = damageWithSpecial * (1 + (totalAffixBonus / 100));
                
                let finalDamage = 0, minDamage = 0, maxDamage = 0;
                
                switch (reaction.type) {
                    case 'catalyze':
                        const skillDamage = (baseDamage * specialMultiplierValue) + this.state.flatDamageBonus;
                        const skillDamageAffix = skillDamage * (1 + (totalAffixBonus / 100));
                        
                        const levelMultiplier = this.getLevelMultiplier(this.state.currentReaction, this.state.globalCharLevel);
                        const emBonusValue = (5 * totalEM) / (totalEM + 1200);
                        const reactionTotalMultiplier = 1 + emBonusValue + reactionBonusValue;
                        const reactionDamage = levelMultiplier * reactionTotalMultiplier;
                        const reactionDamageAffix = reactionDamage * (1 + (totalAffixBonus / 100));
                        
                        const totalBeforeCrit = skillDamageAffix + reactionDamageAffix;
                        const totalWithCrit = totalBeforeCrit * critMultiplier;
                        
                        finalDamage = totalWithCrit * defMultiplier * resMultiplier * directMultiplierValue;
                        minDamage = totalBeforeCrit * defMultiplier * resMultiplier * directMultiplierValue;
                        maxDamage = totalBeforeCrit * (1 + critDmg) * defMultiplier * resMultiplier * directMultiplierValue;
                        break;
                        
                    case 'amplifying':
                    case 'moon_budding':
                        const reactionMultiplier = reaction.type === 'amplifying' ?
                            this.calculateStandardReactionMultiplier(reaction.baseMultiplier, totalEM, this.state.reactionBonus) :
                            this.calculateMoonBuddingMultiplier(reaction.baseMultiplier, totalEM, this.state.reactionBonus);
                        
                        const damageBeforeCrit = damageWithAffix * reactionMultiplier;
                        const damageWithCrit = damageBeforeCrit * critMultiplier;
                        
                        finalDamage = damageWithCrit * defMultiplier * resMultiplier * directMultiplierValue;
                        minDamage = damageBeforeCrit * defMultiplier * resMultiplier * directMultiplierValue;
                        maxDamage = damageBeforeCrit * (1 + critDmg) * defMultiplier * resMultiplier * directMultiplierValue;
                        break;
                        
                    default:
                        const damageCrit = damageWithAffix * critMultiplier;
                        finalDamage = damageCrit * defMultiplier * resMultiplier * directMultiplierValue;
                        minDamage = damageWithAffix * defMultiplier * resMultiplier * directMultiplierValue;
                        maxDamage = damageWithAffix * (1 + critDmg) * defMultiplier * resMultiplier * directMultiplierValue;
                }
                
                return {
                    min: Math.round(minDamage),
                    avg: Math.round(finalDamage),
                    max: Math.round(maxDamage)
                };
            }
            
            calculateDefMultiplier() {
                const reduction = Math.min(this.state.defReduction, 90) / 100;
                const ignore = Math.min(this.state.defIgnore, 100) / 100;
                const numerator = this.state.globalCharLevel + 100;
                const denominator = ((this.state.globalEnemyLevel + 100) * (1 - reduction) * (1 - ignore)) + numerator;
                return numerator / denominator;
            }
            
            calculateResMultiplier() {
                const res = this.state.globalEnemyRes / 100;
                if (res < 0) return 1 - (res / 2);
                if (res >= 0 && res < 0.75) return 1 - res;
                return 1 / (4 * res + 1);
            }
            
            calculateStandardReactionMultiplier(baseMultiplier, em, reactionBonusPercent) {
                const emBonus = (2.78 * em) / (em + 1400);
                const reactionBonusValue = reactionBonusPercent / 100;
                return baseMultiplier * (1 + emBonus + reactionBonusValue);
            }
            
            calculateMoonBuddingMultiplier(baseMultiplier, em, reactionBonusPercent) {
                const emBonus = (6 * em) / (em + 2000);
                const reactionBonusValue = reactionBonusPercent / 100;
                return baseMultiplier * (1 + emBonus + reactionBonusValue);
            }
            
            getLevelMultiplier(reactionType, level) {
                const multipliers = this.LEVEL_MULTIPLIERS[reactionType];
                if (multipliers[level]) return multipliers[level];
                
                const levels = Object.keys(multipliers).map(Number).sort((a, b) => a - b);
                let lower = levels[0], upper = levels[levels.length - 1];
                
                for (let i = 0; i < levels.length - 1; i++) {
                    if (level >= levels[i] && level <= levels[i + 1]) {
                        lower = levels[i];
                        upper = levels[i + 1];
                        break;
                    }
                }
                
                const lowerValue = multipliers[lower];
                const upperValue = multipliers[upper];
                const factor = (level - lower) / (upper - lower);
                return Math.round(lowerValue + (upperValue - lowerValue) * factor);
            }
            
            updateBuildDisplay(buildId, damage) {
                document.getElementById(`minDamage-${buildId}`).textContent = this.formatNumber(damage.min, true);
                document.getElementById(`avgDamage-${buildId}`).textContent = this.formatNumber(damage.avg, true);
                document.getElementById(`maxDamage-${buildId}`).textContent = this.formatNumber(damage.max, true);
                const title = document.getElementById(`damageTitle-${buildId}`);
                if (title) title.textContent = this.REACTIONS[this.state.currentReaction].name.toUpperCase();
            }
            
            showDamageError(buildId) {
                ['min', 'avg', 'max'].forEach(type => {
                    const element = document.getElementById(`${type}Damage-${buildId}`);
                    if (element) {
                        element.textContent = 'Ошибка';
                        element.className = 'damage-value error';
                    }
                });
            }
            
            updateAllBuilds() {
                this.state.builds.forEach(build => this.calculateBuildDamage(build.id));
            }
            
            updateComparisonTable() {
                const tbody = document.getElementById('comparisonBody');
                tbody.innerHTML = '';
                
                if (this.state.builds.length === 0) return;
                
                const sorted = [...this.state.builds].sort((a, b) => b.damage.avg - a.damage.avg);
                const maxDamage = sorted[0].damage.avg;
                
                sorted.forEach((build, index) => {
                    build.isTop = index === 0;
                    if (build.isTop) {
                        build.difference = 0;
                        build.differencePercent = 0;
                    } else {
                        build.difference = maxDamage - build.damage.avg;
                        build.differencePercent = maxDamage > 0 ? (build.difference / maxDamage) * 100 : 0;
                    }
                });
                
                sorted.forEach(build => {
                    const row = document.createElement('tr');
                    if (build.isTop) row.className = 'best-build';
                    
                    row.innerHTML = `
                        <td><strong>${build.name}</strong></td>
                        <td>${this.formatDifference(build.difference, build.differencePercent, build.isTop)}</td>
                        <td>${this.formatNumber(build.damage.min, true)}</td>
                        <td><strong>${this.formatNumber(build.damage.avg, true)}</strong></td>
                        <td>${this.formatNumber(build.damage.max, true)}</td>
                    `;
                    
                    tbody.appendChild(row);
                });
            }
            
            formatDifference(difference, percent, isTop) {
                if (isTop) return '<span class="difference-cell top-build">TOP</span>';
                const diff = this.formatNumber(Math.abs(difference), true);
                const perc = Math.abs(percent).toFixed(1);
                return `<span class="difference-cell difference-negative">
                    <span class="difference-number">-${diff}</span> 
                    <span class="difference-percent">(-${perc}%)</span>
                </span>`;
            }
            
            toggleDualScale() {
                this.state.dualScaleMode = !this.state.dualScaleMode;
                const toggle = document.getElementById('dualScaleToggle');
                
                if (this.state.dualScaleMode) {
                    toggle.classList.add('active');
                    toggle.classList.remove('collapsed');
                    toggle.innerHTML = '<span class="toggle-icon">▼</span> СДВОЕННЫЙ СКЕЙЛ';
                    
                    this.state.builds.forEach(build => {
                        const currentValues = { ...build.values };
                        
                        if (currentValues.skillMultiplier !== undefined) {
                            build.values = {
                                skillMultiplier1: 50,
                                skillMultiplier2: 50,
                                scale1: currentValues.scale || 2000,
                                scale2: currentValues.scale || 2000,
                                critRate: currentValues.critRate || 75,
                                critDmg: currentValues.critDmg || 150,
                                em: currentValues.em || 150,
                                affixBonus: currentValues.affixBonus || 46.6
                            };
                        } else if (currentValues.skillMultiplier1 !== undefined) {
                            build.values.skillMultiplier1 = 50;
                            build.values.skillMultiplier2 = 50;
                            build.values.scale1 = currentValues.scale1 || 2000;
                            build.values.scale2 = currentValues.scale2 || 2000;
                        }
                    });
                } else {
                    toggle.classList.remove('active');
                    toggle.classList.add('collapsed');
                    toggle.innerHTML = '<span class="toggle-icon">▼</span> СДВОЕННЫЙ СКЕЙЛ';
                    
                    this.state.builds.forEach(build => {
                        const currentValues = { ...build.values };
                        
                        build.values = {
                            skillMultiplier: 100,
                            scale: currentValues.scale1 || 2000,
                            critRate: currentValues.critRate || 75,
                            critDmg: currentValues.critDmg || 150,
                            em: currentValues.em || 150,
                            affixBonus: currentValues.affixBonus || 46.6
                        };
                    });
                }
                
                this.rebuildAllBuilds();
            }
            
            rebuildAllBuilds() {
                document.getElementById('buildsContainer').innerHTML = '';
                this.state.builds.forEach(build => {
                    this.createBuildCard(build);
                    this.calculateBuildDamage(build.id);
                });
            }
            
            copyUID() {
                const uid = '728765572';
                navigator.clipboard.writeText(uid).then(() => {
                    const btn = document.getElementById('uidButton');
                    const original = btn.innerHTML;
                    btn.innerHTML = 'Скопировано!';
                    btn.style.background = 'linear-gradient(135deg, #00cc00, #008800)';
                    setTimeout(() => {
                        btn.innerHTML = original;
                        btn.style.background = 'linear-gradient(135deg, var(--green-neon), var(--green-dark))';
                    }, 2000);
                }).catch(() => alert('Скопируйте UID вручную: 728765572'));
            }
            
            resetAll() {
                if (!confirm('Вы уверены, что хотите сбросить все сборки?')) return;
                
                this.state.builds = [];
                this.state.maxBuildId = 0;
                this.state.currentReaction = 'no_reaction';
                this.state.dualScaleMode = false;
                this.state.globalCharLevel = 90;
                this.state.globalEnemyLevel = 95;
                this.state.globalEnemyRes = 10;
                this.state.flatScaleBonus = 0;
                this.state.emBonus = 0;
                this.state.affixBonusBonus = 0;
                this.state.specialMultiplier = 100;
                this.state.flatDamageBonus = 0;
                this.state.reactionBonus = 0;
                this.state.defReduction = 0;
                this.state.defIgnore = 0;
                this.state.directMultiplier = 100;
                
                this.inputConfigs.base.forEach(config => {
                    const element = document.getElementById(config.id);
                    if (element) element.value = config.value;
                });
                
                this.inputConfigs.external.forEach(config => {
                    const element = document.getElementById(config.id);
                    if (element) element.value = config.value;
                });
                
                this.inputConfigs.internal.forEach(config => {
                    const element = document.getElementById(config.id);
                    if (element) element.value = config.value;
                });
                
                document.getElementById('buildsContainer').innerHTML = '';
                document.getElementById('comparisonBody').innerHTML = '';
                
                document.querySelectorAll('.reaction-btn').forEach(btn => btn.classList.remove('active'));
                document.querySelector('[data-reaction="no_reaction"]').classList.add('active');
                
                document.querySelectorAll('.param-toggle-btn').forEach(btn => {
                    btn.classList.add('collapsed');
                    btn.classList.remove('expanded');
                });
                document.querySelectorAll('.params-container, .bonus-container, .internal-bonus-container')
                    .forEach(container => container.classList.remove('visible'));
                
                const dualToggle = document.getElementById('dualScaleToggle');
                dualToggle.classList.remove('active');
                dualToggle.classList.add('collapsed');
                dualToggle.innerHTML = '<span class="toggle-icon">▼</span> СДВОЕННЫЙ СКЕЙЛ';
                
                setTimeout(() => {
                    this.addBuild();
                }, 100);
            }
            
            getDefaultStateValue(key) {
                const defaults = {
                    globalCharLevel: 90, globalEnemyLevel: 95, globalEnemyRes: 10,
                    flatScaleBonus: 0, emBonus: 0, affixBonusBonus: 0,
                    specialMultiplier: 100, flatDamageBonus: 0, reactionBonus: 0,
                    defReduction: 0, defIgnore: 0, directMultiplier: 100,
                    dualScaleMode: false, currentReaction: 'no_reaction'
                };
                return defaults[key] || 0;
            }
        }
    </script>
</body>
</html>
