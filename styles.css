<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CourierFlow | Tracking</title>
    <meta
      name="description"
      content="Modern courier tracking page with live status, ETA, delivery history, and route map."
    />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="container">
      <header class="topbar">
        <div class="brand" aria-label="CourierFlow home">
          <div class="brand-mark">C</div>
          <span>CourierFlow</span>
        </div>

        <nav class="nav" aria-label="Main navigation">
          <a href="#">Home</a>
          <a href="#">Locations</a>
          <a href="#">Support</a>
          <button class="btn secondary">Download app</button>
        </nav>
      </header>

      <main>
        <section class="hero">
          <div class="hero-copy">
            <div class="eyebrow">Live package tracking</div>
            <h1>Track every step from warehouse to doorstep.</h1>
            <p>
              Monitor delivery progress in real time, view shipment history,
              and stay informed with accurate ETA updates across the entire route.
            </p>

            <div class="hero-actions">
              <button class="btn primary" onclick="document.getElementById('trackingInput').focus()">
                Track shipment
              </button>
              <button class="btn secondary">Get alerts</button>
            </div>
          </div>

          <div class="tracking-panel">
            <div class="small-label">Tracking number</div>

            <form class="track-form" id="trackingForm">
              <input
                id="trackingInput"
                type="text"
                value="CF-2847-9001"
                placeholder="Enter tracking code"
                aria-label="Tracking number"
              />
              <button type="submit">Track</button>
            </form>

            <div class="status-summary">
              <div class="status-line">
                <div class="status-badge">
                  <span class="dot"></span>
                  <span id="statusBadgeText">In transit</span>
                </div>
                <div class="chip" id="shipmentId">CF-2847-9001</div>
              </div>

              <div class="eta">
                <strong id="etaValue">2</strong>
                <span>days remaining</span>
              </div>
            </div>

            <div class="info-grid">
              <div class="mini-card">
                <div class="label">Origin</div>
                <div class="value" id="originName">Seattle, USA</div>
              </div>
              <div class="mini-card">
                <div class="label">Destination</div>
                <div class="value" id="destinationName">Austin, USA</div>
              </div>
              <div class="mini-card">
                <div class="label">Last update</div>
                <div class="value" id="lastUpdate">Today, 8:20 AM</div>
              </div>
            </div>
          </div>
        </section>

        <section class="main-section">
          <div class="panel map-panel">
            <div class="panel-header">
              <div class="panel-title">Route map</div>
              <div class="chip" id="routeProgress">78% complete</div>
            </div>

            <div class="map" aria-label="Courier route map">
              <div class="route-line"></div>

              <div class="map-dot origin"></div>
              <div class="map-dot hub stopped"></div>
              <div class="map-dot location"></div>
              <div class="map-dot destination"></div>

              <div class="route-labels">
                <span class="origin-tag">Origin</span>
                <span class="hub-tag">Hub</span>
                <span class="current-tag">Current</span>
                <span class="dest-tag">Destination</span>
              </div>
            </div>

            <div class="route-legend">
              <div class="legend-item"><span class="legend-dot"></span> In transit</div>
              <div class="legend-item"><span class="legend-dot green"></span> Delivered</div>
              <div class="legend-item"><span class="legend-dot yellow"></span> Alert / delay</div>
            </div>
          </div>

          <aside class="panel details-panel">
            <div class="panel-header">
              <div class="panel-title">Shipment details</div>
              <div class="chip">Priority</div>
            </div>

            <div class="summary-box">
              <h3>Package overview</h3>
              <div class="detail-list">
                <div class="detail-row">
                  <span class="key">Courier</span>
                  <span class="value" id="courierValue">CourierFlow Express</span>
                </div>
                <div class="detail-row">
                  <span class="key">Weight</span>
                  <span class="value" id="weightValue">4.8 kg</span>
                </div>
                <div class="detail-row">
                  <span class="key">ETA</span>
                  <span class="value" id="etaDetail">Thu, 5:30 PM</span>
                </div>
                <div class="detail-row">
                  <span class="key">Recipient</span>
                  <span class="value" id="recipientValue">Olivia M.</span>
                </div>
              </div>
            </div>

            <button type="button" class="notify" id="notifyButton">
              <span>🔔</span>
              Enable notifications
            </button>
          </aside>
        </section>

        <section class="panel timeline-panel">
          <div class="panel-header">
            <div class="panel-title">Delivery history</div>
            <div class="chip">Updated live</div>
          </div>

          <div class="timeline" id="timeline"></div>
        </section>
      </main>
    </div>

    <div class="toast" id="toast" aria-live="polite"></div>

    <script src="script.js"></script>
  </body>
</html>
