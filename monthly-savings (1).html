<!-- Monthly Savings Tracker -->
<div id="app-root"></div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>
<style>
  #app-root, #app-root * { box-sizing: border-box; }
  #app-root {
    --pink: #ec5f8e;
    --pink-soft: #fbc7d4;
    --blue: #5b9bd9;
    --blue-soft: #bcdcf7;
    --green: #59b48a;
    --purple: #9b7fd4;
    --cream: #fff8f0;
    --ink: #3a2e35;
    --muted: #9a8b93;
    font-family: 'Segoe UI', -apple-system, BlinkMacSystemFont, sans-serif;
    color: var(--ink);
    max-width: 760px;
    margin: 0 auto;
    padding: 12px;
    background: var(--cream);
  }
  .banner {
    background: linear-gradient(120deg, #f492b0, #f7c9a0 55%, #bcdcf7);
    border-radius: 22px;
    padding: 22px 26px;
    display: flex;
    align-items: center;
    gap: 18px;
    position: relative;
    overflow: hidden;
    margin-bottom: 16px;
  }
  .banner .piggy {
    width: 54px; height: 54px; border-radius: 16px;
    background: rgba(255,255,255,0.6);
    display: flex; align-items: center; justify-content: center;
    font-size: 28px; flex-shrink: 0;
  }
  .banner h1 { margin: 0; font-size: 22px; font-weight: 800; color: #c0396a; }
  .banner p { margin: 2px 0 8px; font-size: 13px; color: #7a5b60; }
  .year-nav { display: flex; align-items: center; gap: 10px; }
  .year-nav button {
    width: 28px; height: 28px; border-radius: 50%; border: none;
    background: rgba(255,255,255,0.75); font-size: 15px; cursor: pointer;
    color: #c0396a; font-weight: 700;
  }
  .year-nav span { font-weight: 800; font-size: 15px; }

  .people-row { display: flex; gap: 8px; flex-wrap: wrap; margin-bottom: 14px; align-items: center; }
  .chip {
    display: flex; align-items: center; gap: 8px;
    padding: 7px 14px; border-radius: 999px; color: #fff; font-weight: 700; font-size: 14px;
  }
  .chip button {
    background: rgba(255,255,255,0.35); border: none; color: #fff;
    width: 18px; height: 18px; border-radius: 50%; cursor: pointer; font-size: 11px; line-height: 1;
  }
  .chip-add {
    width: 36px; height: 36px; border-radius: 50%; border: 2px dashed var(--pink);
    background: transparent; color: var(--pink); font-size: 18px; cursor: pointer;
  }

  table { width: 100%; border-collapse: collapse; background: #fffdfb; border-radius: 16px; overflow: hidden; box-shadow: 0 2px 10px rgba(0,0,0,0.04); }
  thead th { text-align: right; padding: 12px 14px; font-size: 12px; color: var(--muted); border-bottom: 1px solid #f1e6e4; }
  thead th:first-child { text-align: left; }
  thead th.total-col { color: var(--pink); }
  tbody td { padding: 12px 14px; text-align: right; font-size: 14px; border-bottom: 1px solid #f6efed; }
  tbody td:first-child { text-align: left; display: flex; align-items: center; gap: 8px; font-weight: 600; }
  .dot { width: 8px; height: 8px; border-radius: 50%; background: #d8d0d3; flex-shrink: 0; }
  .dot.filled { background: var(--green); }
  tr:nth-child(even) td { background: #fffaf6; }
  .cell-edit { cursor: pointer; border-radius: 6px; padding: 2px 4px; transition: background .1s; }
  .cell-edit:hover { background: #fbeef2; }
  .cell-input { width: 70px; text-align: right; border: 1px solid var(--pink); border-radius: 6px; padding: 3px 6px; font-size: 14px; }
  .total-cell { color: var(--pink); font-weight: 700; }
  tfoot td { padding: 12px 14px; text-align: right; font-weight: 800; font-size: 14px; }
  tfoot td:first-child { text-align: left; color: var(--pink); }
  .grand-row td { background: linear-gradient(90deg, #f492b0, #ec5f8e); color: #fff; padding: 14px; border-radius: 0 0 16px 16px; }
  .grand-row td:first-child { border-radius: 0 0 0 16px; }
  .grand-row td:last-child { border-radius: 0 0 16px 0; }

  .stats { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin: 16px 0; }
  .stat-card { background: #fffdfb; border-radius: 14px; padding: 14px 16px; box-shadow: 0 2px 8px rgba(0,0,0,0.03); }
  .stat-label { font-size: 11px; color: var(--muted); text-transform: uppercase; font-weight: 700; letter-spacing: .04em; margin-bottom: 4px; }
  .stat-value { font-size: 22px; font-weight: 800; }
  .stat-sub { font-size: 12px; color: var(--muted); margin-top: 2px; }

  .notes-title { font-weight: 800; font-size: 16px; margin: 18px 0 10px; display: flex; align-items: center; gap: 6px; }
  .note {
    background: #fff8ef; border-radius: 12px; padding: 12px 14px; margin-bottom: 8px;
    display: flex; justify-content: space-between; align-items: center; gap: 10px; font-size: 14px;
  }
  .note button { background: none; border: none; color: #c9a; cursor: pointer; font-size: 14px; opacity: .6; }
  .add-note {
    width: 100%; border: 2px dashed var(--blue); background: transparent; color: var(--blue);
    border-radius: 12px; padding: 12px; font-weight: 700; cursor: pointer; font-size: 14px;
  }

  .toolbar { display: flex; gap: 8px; margin: 14px 0; flex-wrap: wrap; }
  .btn { border: none; border-radius: 10px; padding: 9px 14px; font-weight: 700; font-size: 13px; cursor: pointer; }
  .btn-primary { background: var(--pink); color: #fff; }
  .btn-ghost { background: #fff; color: var(--pink); border: 1px solid var(--pink-soft); }

  .toast-wrap { position: fixed; top: 16px; left: 50%; transform: translateX(-50%); z-index: 999; display: flex; flex-direction: column; gap: 8px; align-items: center; }
  .toast {
    background: #3a2e35; color: #fff; padding: 10px 18px; border-radius: 999px; font-size: 13px;
    box-shadow: 0 4px 14px rgba(0,0,0,0.2); animation: fadein .2s ease-out;
  }
  @keyframes fadein { from { opacity: 0; transform: translateY(-8px); } to { opacity: 1; transform: translateY(0); } }

  .footnote { font-size: 12px; color: var(--muted); text-align: center; margin: 18px 0 6px; line-height: 1.5; }
</style>

<script type="text/babel" data-presets="react">
const { useState, useEffect, useRef, useCallback } = React;

const MONTHS = ["January","February","March","April","May","June","July","August","September","October","November","December"];
const PALETTE = ["#ec5f8e", "#5b9bd9", "#59b48a", "#9b7fd4", "#e0a13c", "#4fb3bf"];
const STORAGE_KEY = "monthly-savings-data";
const money = n => "\u20B1" + Number(n||0).toLocaleString();

function defaultData() {
  return {
    people: ["Reyma", "Dave"],
    years: {
      2026: {
        entries: {
          January: {Reyma:0, Dave:0}, February: {Reyma:0, Dave:0},
          March: {Reyma:3000, Dave:3000}, April: {Reyma:3000, Dave:4000},
          May: {Reyma:3000, Dave:3000}, June: {Reyma:3000, Dave:3000}
        },
        notes: [
          "Tip: tap any amount to edit it. Tap the trash icon to remove a note.",
          "April 2026: 10k for bahay ng baboy at patubig",
          "May 2026: 2k feeds",
          "June 2026: Cat need 683 pesos"
        ]
      }
    }
  };
}

function App() {
  const [data, setData] = useState(null);
  const [year, setYear] = useState(2026);
  const [toasts, setToasts] = useState([]);
  const [notifPermission, setNotifPermission] = useState(
    (typeof Notification !== "undefined") ? Notification.permission : "unsupported"
  );
  const [editingCell, setEditingCell] = useState(null); // {month, person}
  const [editValue, setEditValue] = useState("");
  const exportRef = useRef(null);
  const [exporting, setExporting] = useState(false);
  const saveTimer = useRef(null);

  const notify = useCallback((title, body) => {
    const id = Date.now() + Math.random();
    setToasts(t => [...t, {id, title, body}]);
    setTimeout(() => setToasts(t => t.filter(x => x.id !== id)), 3200);
    if (typeof Notification !== "undefined" && Notification.permission === "granted") {
      try { new Notification(title, {body}); } catch(e) {}
    }
  }, []);

  useEffect(() => {
    (async () => {
      try {
        const res = await window.storage.get(STORAGE_KEY, true);
        setData(res && res.value ? JSON.parse(res.value) : defaultData());
      } catch (e) {
        setData(defaultData());
      }
    })();
  }, []);

  const persist = useCallback((next) => {
    setData(next);
    if (saveTimer.current) clearTimeout(saveTimer.current);
    saveTimer.current = setTimeout(async () => {
      try {
        await window.storage.set(STORAGE_KEY, JSON.stringify(next), true);
      } catch (e) {
        notify("Couldn't save", "Your change may not have synced. Try again.");
      }
    }, 250);
  }, [notify]);

  if (!data) {
    return <div style={{padding: "40px", textAlign: "center", color: "#9a8b93"}}>Loading your piggy bank…</div>;
  }

  const yearData = data.years[year] || { entries: {}, notes: [] };
  const people = data.people;

  const colorFor = (name) => PALETTE[people.indexOf(name) % PALETTE.length];

  const monthTotal = (month) => {
    const e = yearData.entries[month];
    if (!e) return null;
    return people.reduce((s,p) => s + (Number(e[p])||0), 0);
  };

  const personTotal = (person) => {
    return MONTHS.reduce((s,m) => {
      const e = yearData.entries[m];
      return s + (e ? (Number(e[person])||0) : 0);
    }, 0);
  };

  const grandTotal = people.reduce((s,p) => s + personTotal(p), 0);
  const monthsWithAmount = MONTHS.map(m => ({m, t: monthTotal(m)})).filter(x => x.t);
  const bestMonth = monthsWithAmount.reduce((best,cur) => (!best || cur.t > best.t) ? cur : best, null);
  const monthlyAvg = monthsWithAmount.length ? Math.round(grandTotal / monthsWithAmount.length) : 0;
  const topSaver = people.reduce((best,p) => {
    const t = personTotal(p);
    return (!best || t > best.t) ? {p, t} : best;
  }, null);

  const addYearIfMissing = (y, next) => {
    if (!next.years[y]) next.years[y] = { entries: {}, notes: [] };
  };

  const changeYear = (delta) => {
    const ny = year + delta;
    const next = JSON.parse(JSON.stringify(data));
    addYearIfMissing(ny, next);
    persist(next);
    setYear(ny);
  };

  const addPerson = () => {
    const name = prompt("Name of the new saver:");
    if (!name || !name.trim()) return;
    if (people.includes(name.trim())) { notify("Already added", `${name} is already on the list.`); return; }
    const next = JSON.parse(JSON.stringify(data));
    next.people.push(name.trim());
    persist(next);
    notify("Saver added", `${name.trim()} can now track their savings.`);
  };

  const removePerson = (name) => {
    if (!confirm(`Remove ${name} and their saved amounts?`)) return;
    const next = JSON.parse(JSON.stringify(data));
    next.people = next.people.filter(p => p !== name);
    Object.values(next.years).forEach(y => {
      Object.values(y.entries).forEach(e => { delete e[name]; });
    });
    persist(next);
  };

  const openCellEditor = (month, person) => {
    const e = yearData.entries[month];
    const current = e && e[person] !== undefined ? e[person] : "";
    setEditingCell({month, person});
    setEditValue(String(current));
  };

  const commitCell = () => {
    if (!editingCell) return;
    const { month, person } = editingCell;
    const val = editValue.trim() === "" ? 0 : Math.max(0, Number(editValue) || 0);
    const next = JSON.parse(JSON.stringify(data));
    addYearIfMissing(year, next);
    if (!next.years[year].entries[month]) next.years[year].entries[month] = {};
    next.years[year].entries[month][person] = val;
    persist(next);
    setEditingCell(null);
    notify("Saved", `${person} · ${month}: ${money(val)}`);
  };

  const resetCell = (month, person) => {
    const e = yearData.entries[month];
    if (!e) return;
    const next = JSON.parse(JSON.stringify(data));
    delete next.years[year].entries[month][person];
    if (Object.keys(next.years[year].entries[month]).length === 0) {
      delete next.years[year].entries[month];
    }
    persist(next);
  };

  const addNote = () => {
    const text = prompt("Add a note:");
    if (!text || !text.trim()) return;
    const next = JSON.parse(JSON.stringify(data));
    addYearIfMissing(year, next);
    next.years[year].notes.push(text.trim());
    persist(next);
  };

  const removeNote = (idx) => {
    const next = JSON.parse(JSON.stringify(data));
    next.years[year].notes.splice(idx, 1);
    persist(next);
  };

  const requestNotifPermission = async () => {
    if (typeof Notification === "undefined") {
      notify("Not supported here", "This browser/embed doesn't allow device notifications, so you'll get in-app alerts instead.");
      return;
    }
    const perm = await Notification.requestPermission();
    setNotifPermission(perm);
    if (perm === "granted") {
      notify("Notifications on", "You'll get a device alert whenever an amount is saved.");
    } else {
      notify("Notifications off", "You'll still see in-app alerts here.");
    }
  };

  const exportImage = async () => {
    setExporting(true);
    try {
      const canvas = await html2canvas(exportRef.current, {
        backgroundColor: "#fff8f0", scale: 2, useCORS: true
      });
      const link = document.createElement("a");
      link.download = `monthly-savings-${year}.png`;
      link.href = canvas.toDataURL("image/png");
      link.click();
      notify("Image saved", "Downloaded to your device.");
    } catch (e) {
      notify("Export failed", "Try again in a moment.");
    }
    setExporting(false);
  };

  return (
    <div>
      <div className="toast-wrap">
        {toasts.map(t => (
          <div className="toast" key={t.id}><strong>{t.title}</strong>{t.body ? " — " + t.body : ""}</div>
        ))}
      </div>

      <div ref={exportRef}>
        <div className="banner">
          <div className="piggy">🐷</div>
          <div style={{flex:1}}>
            <h1>Monthly Savings</h1>
            <p>Your piggy bank is ready!</p>
            <div className="year-nav">
              <button onClick={() => changeYear(-1)}>‹</button>
              <span>{year}</span>
              <button onClick={() => changeYear(1)}>›</button>
            </div>
          </div>
        </div>

        <div className="people-row">
          {people.map(p => (
            <div className="chip" style={{background: colorFor(p)}} key={p}>
              {p}
              <button onClick={() => removePerson(p)}>✕</button>
            </div>
          ))}
          <button className="chip-add" onClick={addPerson} title="Add a saver">+</button>
        </div>

        <table>
          <thead>
            <tr>
              <th>Month</th>
              {people.map(p => <th key={p}>{p}</th>)}
              <th className="total-col">Total</th>
            </tr>
          </thead>
          <tbody>
            {MONTHS.map(month => {
              const e = yearData.entries[month];
              const hasData = !!e;
              return (
                <tr key={month}>
                  <td><span className={"dot" + (hasData ? " filled" : "")}></span>{month}</td>
                  {people.map(p => {
                    const isEditing = editingCell && editingCell.month === month && editingCell.person === p;
                    const val = e && e[p] !== undefined ? e[p] : null;
                    return (
                      <td key={p}>
                        {isEditing ? (
                          <input
                            className="cell-input"
                            autoFocus
                            type="number"
                            value={editValue}
                            onChange={ev => setEditValue(ev.target.value)}
                            onBlur={commitCell}
                            onKeyDown={ev => { if (ev.key === "Enter") commitCell(); if (ev.key === "Escape") setEditingCell(null); }}
                          />
                        ) : (
                          <span
                            className="cell-edit"
                            onClick={() => openCellEditor(month, p)}
                            onContextMenu={ev => { ev.preventDefault(); resetCell(month, p); }}
                            title="Tap to edit · right-click to clear"
                          >
                            {val === null ? "—" : val}
                          </span>
                        )}
                      </td>
                    );
                  })}
                  <td className="total-cell">{monthTotal(month) === null ? "₱0" : money(monthTotal(month))}</td>
                </tr>
              );
            })}
          </tbody>
          <tfoot>
            <tr>
              <td>Total</td>
              {people.map(p => <td key={p}>{money(personTotal(p))}</td>)}
              <td>{money(grandTotal)}</td>
            </tr>
            <tr className="grand-row">
              <td>Grand Total</td>
              <td colSpan={people.length + 1}>{money(grandTotal)}</td>
            </tr>
          </tfoot>
        </table>

        <div className="stats">
          <div className="stat-card">
            <div className="stat-label">💰 Total Savings</div>
            <div className="stat-value" style={{color: "var(--pink)"}}>{money(grandTotal)}</div>
            <div className="stat-sub">Year to date</div>
          </div>
          <div className="stat-card">
            <div className="stat-label">🏆 Top Saver</div>
            <div className="stat-value" style={{color: topSaver ? colorFor(topSaver.p) : "var(--ink)"}}>{topSaver ? topSaver.p : "—"}</div>
            <div className="stat-sub">{topSaver ? `${money(topSaver.t)} saved` : "No data yet"}</div>
          </div>
          <div className="stat-card">
            <div className="stat-label">📊 Best Month</div>
            <div className="stat-value" style={{color: "#e0a13c"}}>{bestMonth ? bestMonth.m.slice(0,3) : "—"}</div>
            <div className="stat-sub">{bestMonth ? money(bestMonth.t) : "No data yet"}</div>
          </div>
          <div className="stat-card">
            <div className="stat-label">📈 Monthly Avg</div>
            <div className="stat-value" style={{color: "var(--green)"}}>{money(monthlyAvg)}</div>
            <div className="stat-sub">Across {monthsWithAmount.length} month(s)</div>
          </div>
        </div>

        <div className="notes-title">📋 Notes &amp; Adjustments</div>
        {(yearData.notes || []).map((n, i) => (
          <div className="note" key={i}>
            <span>{n}</span>
            <button onClick={() => removeNote(i)}>🗑</button>
          </div>
        ))}
        <button className="add-note" onClick={addNote}>+ Add a note</button>
      </div>

      <div className="toolbar">
        <button className="btn btn-primary" onClick={exportImage} disabled={exporting}>
          {exporting ? "Saving…" : "⬇ Save as image"}
        </button>
        <button className="btn btn-ghost" onClick={requestNotifPermission}>
          {notifPermission === "granted" ? "🔔 Notifications on" : "🔕 Turn on notifications"}
        </button>
      </div>

      <div className="footnote">
        Data is shared and synced for everyone who opens this — publish this artifact to get a link that works on any phone, tablet, or computer.<br/>
        Device notifications need your browser's permission; if it's blocked, you'll still see in-app alerts here.
      </div>
    </div>
  );
}

ReactDOM.createRoot(document.getElementById("app-root")).render(<App />);
</script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react/18.3.1/umd/react.production.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/18.3.1/umd/react-dom.production.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/7.24.7/babel.min.js"></script>
