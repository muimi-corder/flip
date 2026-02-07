<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <title>激ムズ！ペットボトルフリップ</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/matter-js/0.19.0/matter.min.js"></script>
    <style>
        body { margin: 0; overflow: hidden; background: #f0f0f0; font-family: sans-serif; }
        #ui { position: absolute; top: 20px; left: 20px; pointer-events: none; }
    </style>
</head>
<body>
    <div id="ui">
        <h1>Bottle Flip Proto</h1>
        <p>マウスで掴んで投げてみよう！</p>
    </div>
    <script>
        const { Engine, Render, Runner, Bodies, Composite, MouseConstraint, Mouse, Events } = Matter;

        // エンジンと描画の設定
        const engine = Engine.create();
        const render = Render.create({
            element: document.body,
            engine: engine,
            options: {
                width: window.innerWidth,
                height: window.innerHeight,
                wireframes: false,
                background: '#e0e0e0'
            }
        });

        // 床の作成
        const ground = Bodies.rectangle(window.innerWidth/2, window.innerHeight - 50, window.innerWidth, 100, { 
            isStatic: true, 
            render: { fillStyle: '#888' } 
        });

        // ペットボトルの作成（少し重心を下にするためにカスタム）
        const bottle = Bodies.rectangle(window.innerWidth/2, window.innerHeight - 150, 60, 150, {
            friction: 0.5,
            restitution: 0.3, // 跳ね返り
            density: 0.001,
            render: { fillStyle: '#3498db', strokeStyle: '#2980b9', lineWidth: 5 }
        });

        // マウス操作の追加
        const mouse = Mouse.create(render.canvas);
        const mouseConstraint = MouseConstraint.create(engine, {
            mouse: mouse,
            constraint: { stiffness: 0.2, render: { visible: false } }
        });

        // 世界にオブジェクトを追加
        Composite.add(engine.world, [ground, bottle, mouseConstraint]);

        // 実行
        Render.run(render);
        const runner = Runner.create();
        Runner.run(runner, engine);

        // 画面リサイズ対応
        window.addEventListener('resize', () => {
            render.canvas.width = window.innerWidth;
            render.canvas.height = window.innerHeight;
        });
    </script>
</body>
</html>
