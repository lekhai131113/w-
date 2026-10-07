# <!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Độ nhạy kéo tâm Free Fire | Tối ưu</title>
    <style>
        /* Reset & base */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: #0a0a0a;
            color: #e0e0e0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 2rem 1rem;
            line-height: 1.5;
        }

        /* main card container – bo góc lớn, nền đen, viền trắng mảnh */
        .card {
            background: #111111;
            border: 1px solid #2a2a2a;
            border-radius: 42px;
            padding: 2rem 2.2rem;
            max-width: 1100px;
            width: 100%;
            box-shadow: 0 25px 40px -12px rgba(0, 0, 0, 0.8), 0 0 0 1px rgba(255, 255, 255, 0.02);
            transition: all 0.2s;
        }

        /* Tiêu đề chính */
        h1 {
            font-size: 2.6rem;
            font-weight: 700;
            letter-spacing: -0.02em;
            color: #ffffff;
            display: flex;
            align-items: center;
            gap: 0.75rem;
            border-bottom: 1px solid #2a2a2a;
            padding-bottom: 1.2rem;
            margin-bottom: 2rem;
            text-transform: uppercase;
        }

        h1 span {
            background: #ffffff;
            color: #0a0a0a;
            font-size: 1.2rem;
            font-weight: 600;
            padding: 0.2rem 1rem;
            border-radius: 100px;
            letter-spacing: 0.5px;
            margin-left: 0.5rem;
        }

        /* Lưới các mẹo – dạng grid bo góc */
        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 1.5rem;
            margin-bottom: 2.5rem;
        }

        /* Thẻ mẹo – bo góc mềm, nền đen, viền trắng mờ */
        .tip-card {
            background: #0c0c0c;
            border: 1px solid #2e2e2e;
            border-radius: 28px;
            padding: 1.5rem 1.4rem;
            transition: 0.25s ease;
            box-shadow: 0 8px 0 #000000;
        }

        .tip-card:hover {
            border-color: #5a5a5a;
            background: #151515;
            transform: translateY(-3px);
            box-shadow: 0 12px 0 #000000;
        }

        /* số thứ tự hoặc icon */
        .tip-number {
            display: inline-block;
            background: #ffffff;
            color: #0a0a0a;
            font-weight: 700;
            font-size: 0.9rem;
            width: 32px;
            height: 32px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 12px;
            margin-bottom: 1.2rem;
            letter-spacing: -0.3px;
        }

        .tip-card h3 {
            font-size: 1.25rem;
            font-weight: 600;
            color: #ffffff;
            margin-bottom: 0.5rem;
            letter-spacing: -0.02em;
        }

        .tip-card p {
            font-size: 0.95rem;
            color: #a0a0a0;
            line-height: 1.5;
        }

        /* Phần độ nhạy chi tiết – bảng bo góc */
        .sensitivity-section {
            background: #0c0c0c;
            border: 1px solid #2e2e2e;
            border-radius: 32px;
            padding: 1.8rem 2rem;
            margin-top: 0.5rem;
            box-shadow: 0 8px 0 #000000;
        }

        .sensitivity-header {
            display: flex;
            align-items: center;
            gap: 0.8rem;
            margin-bottom: 1.8rem;
            flex-wrap: wrap;
        }

        .sensitivity-header h2 {
            font-size: 1.7rem;
            font-weight: 600;
            color: #ffffff;
            letter-spacing: -0.02em;
        }

        .sensitivity-header .badge {
            background: #ffffff;
            color: #0a0a0a;
            font-size: 0.8rem;
            font-weight: 600;
            padding: 0.25rem 0.9rem;
            border-radius: 50px;
            text-transform: uppercase;
        }

        .sensitivity-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
            gap: 1.2rem;
        }

        .sensitivity-item {
            background: #111111;
            border-radius: 24px;
            padding: 1.2rem 0.8rem;
            text-align: center;
            border: 1px solid #2a2a2a;
            transition: all 0.2s;
        }

        .sensitivity-item:hover {
            background: #1a1a1a;
            border-color: #4a4a4a;
        }

        .sensitivity-label {
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-weight: 500;
            color: #8a8a8a;
            margin-bottom: 0.6rem;
        }

        .sensitivity-value {
            font-size: 2.1rem;
            font-weight: 800;
            color: #ffffff;
            line-height: 1.2;
            letter-spacing: -0.03em;
        }

        .sensitivity-note {
            margin-top: 1.8rem;
            font-size: 0.9rem;
            color: #888;
            background: #0a0a0a;
            padding: 0.9rem 1.4rem;
            border-radius: 60px;
            border: 1px solid #252525;
            display: inline-block;
            width: auto;
        }

        /* Nút giả lập / ghi chú thêm */
        .extra-note {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-between;
            margin-top: 2rem;
            padding-top: 1.5rem;
            border-top: 1px solid #252525;
            font-size: 0.9rem;
            color: #7a7a7a;
        }

        .extra-note .highlight {
            color: #ffffff;
            font-weight: 500;
            background: #1f1f1f;
            padding: 0.3rem 1.2rem;
            border-radius: 40px;
            border: 1px solid #333;
        }

        /* responsive */
        @media (max-width: 600px) {
            .card {
                padding: 1.5rem 1.2rem;
                border-radius: 32px;
            }
            h1 {
                font-size: 1.8rem;
                flex-wrap: wrap;
            }
            h1 span {
                font-size: 0.9rem;
                margin-left: 0;
            }
            .sensitivity-section {
                padding: 1.4rem 1rem;
            }
            .sensitivity-value {
                font-size: 1.7rem;
            }
        }

        /* custom scrollbar cho đẹp */
        ::-webkit-scrollbar {
            width: 8px;
            background: #111;
        }
        ::-webkit-scrollbar-thumb {
            background: #333;
            border-radius: 20px;
        }
    </style>
</head>
<body>
    <div class="card">
        <!-- Tiêu đề chính -->
        <h1>
            Độ nhạy kéo tâm
            <span>FREE FIRE</span>
        </h1>

        <!-- Lưới các mẹo kéo tâm -->
        <div class="tips-grid">
            <div class="tip-card">
                <div class="tip-number">01</div>
                <h3>Kéo tâm từ dưới lên</h3>
                <p>Bắt đầu từ phần dưới mục tiêu, kéo nhẹ lên theo đường thẳng. Giữ lực đều tay, tránh giật cục.</p>
            </div>
            <div class="tip-card">
                <div class="tip-number">02</div>
                <h3>Luyện tập ở bãi tập</h3>
                <p>Dành 10–15 phút mỗi ngày ở Training Ground để làm quen với độ nhạy và cảm giác kéo tâm.</p>
            </div>
            <div class="tip-card">
                <div class="tip-number">03</div>
                <h3>Dùng ngón cái & ngón trỏ</h3>
                <p>Phối hợp ngón cái giữ màn hình, ngón trỏ kéo tâm giúp kiểm soát tốt hơn, đặc biệt khi bắn tỉa.</p>
            </div>
            <div class="tip-card">
                <div class="tip-number">04</div>
                <h3>Điều chỉnh theo súng</h3>
                <p>Súng có độ giật khác nhau. MP40 cần kéo nhẹ, AK lại cần kéo mạnh và dứt khoát hơn.</p>
            </div>
            <div class="tip-card">
                <div class="tip-number">05</div>
                <h3>Kéo tâm theo hình chữ U</h3>
                <p>Khi địch di chuyển ngang, kéo tâm theo hình chữ U để bám sát mục tiêu, tránh bị lệch.</p>
            </div>
            <div class="tip-card">
                <div class="tip-number">06</div>
                <h3>Tận dụng gyro (nếu có)</h3>
                <p>Bật gyro ở mức thấp đến trung bình, kết hợp kéo tâm bằng tay để tăng độ chính xác khi xả đạn.</p>
            </div>
        </div>

        <!-- Phần độ nhạy chi tiết -->
        <div class="sensitivity-section">
            <div class="sensitivity-header">
                <h2>Thông số độ nhạy</h2>
                <div class="badge">Tối ưu</div>
            </div>

            <div class="sensitivity-grid">
                <div class="sensitivity-item">
                    <div class="sensitivity-label">Tổng quát</div>
                    <div class="sensitivity-value">85</div>
                </div>
                <div class="sensitivity-item">
                    <div class="sensitivity-label">Điểm đỏ</div>
                    <div class="sensitivity-value">78</div>
                </div>
                <div class="sensitivity-item">
                    <div class="sensitivity-label">2x</div>
                    <div class="sensitivity-value">72</div>
                </div>
                <div class="sensitivity-item">
                    <div class="sensitivity-label">4x</div>
                    <div class="sensitivity-value">65</div>
                </div>
                <div class="sensitivity-item">
                    <div class="sensitivity-label">AWM</div>
                    <div class="sensitivity-value">60</div>
                </div>
                <div class="sensitivity-item">
                    <div class="sensitivity-label">Free look</div>
                    <div class="sensitivity-value">70</div>
                </div>
            </div>

            <div class="sensitivity-note">
                ⚡ Độ nhạy kéo tâm tối ưu: <strong>85 – 95</strong> (tùy thiết bị)
            </div>
        </div>

        <!-- Ghi chú thêm -->
        <div class="extra-note">
            <span>🎯 Mẹo: Kéo tâm mượt mà hơn khi để độ nhạy tổng quát cao.</span>
            <span class="highlight">#FreeFire #KéoTâm</span>
        </div>
    </div>
</body>
</html>w-