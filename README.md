graph TD
    %% 定义区域样式
    classDef uncontrol fill:#f5f5f5,stroke:#666,stroke-width:1px;
    classDef areaC fill:#e1f5fe,stroke:#01579b,stroke-width:2px;
    classDef areaB fill:#fff9c4,stroke:#fbc02d,stroke-width:2px;

    subgraph 非受控区_准备段
    A[脱外鞋] --> B[更换拖鞋]
    B --> C[手消]
    end

    subgraph C级洁净区_更衣程序
    C --> D[更换C区拖鞋]:::areaC
    D --> E[穿戴头套/口罩/手套]:::areaC
    E --> F[穿戴C区洁净服]:::areaC
    F --> G[进入C区通道/功能间]:::areaC
    end

    subgraph B级洁净区_更衣程序
    G --> H[更换B区拖鞋]:::areaB
    H --> I[穿戴B区洁净服]:::areaB
    I --> J[穿戴第二层手套]:::areaB
    J --> K[进入B级核心区]:::areaB
    end

    %% 指示说明
    class A,B,C uncontrol;
