# FTS
Author - Sunny Shah

<!-- . -->
<!-- import { useEffect } from "react";

export default function Sidebar({ isOpen, onClose }) {
  useEffect(() => {
    if (isOpen) {
      document.body.classList.add("overflow-hidden");
      history.pushState({ sidebarOpen: true }, "");
    } else {
      document.body.classList.remove("overflow-hidden");
    }

    const handlePopState = () => {
      if (isOpen) onClose();
    };

    const handleKeyDown = (e) => {
      if (e.key === "Escape") onClose();
    };

    window.addEventListener("popstate", handlePopState);
    window.addEventListener("keydown", handleKeyDown);

    return () => {
      window.removeEventListener("popstate", handlePopState);
      window.removeEventListener("keydown", handleKeyDown);
    };
  }, [isOpen, onClose]);

  const handleOverlayClick = (e) => {
    if (e.target.id === "overlay") onClose();
  };

  return (
    <>
      {/* Overlay */}
      <div
        id="overlay"
        onClick={handleOverlayClick}
        className={`fixed inset-0 bg-black bg-opacity-60 z-[999] transition-opacity duration-300 ${
          isOpen ? "opacity-100 visible" : "opacity-0 invisible"
        }`}
      />

      {/* Sidebar */}
      <div
        className={`fixed top-0 left-0 bottom-0 w-80 bg-white z-[1000] transform transition-transform duration-300 ${
          isOpen ? "translate-x-0" : "-translate-x-full"
        } shadow-xl overflow-auto`}
      >
        <div className="sticky top-0 bg-white border-b py-4 px-4">
          <h2 className="text-lg font-semibold">Menu</h2>
        </div>
        <ul className="mt-4 mx-4 space-y-2">
          <li>🏠 Home</li>
          <li>🛒 Grocery</li>
          <li>🍀 Organic Foods</li>
          <li>🧺 Laundry</li>
          <li>🧼 Cleaning</li>
          <li>📚 Stationery</li>
          <li>👗 Fashion</li>
          <li>💄 Cosmetic</li>
          <li>🧻 Sanitary</li>
        </ul>
      </div>
    </>
  );
}




import { useState } from "react";
import Sidebar from "./components/Sidebar";

function App() {
  const [isSidebarOpen, setSidebarOpen] = useState(false);

  return (
    <div className="relative">
      <header className="p-4 bg-red-500 text-white flex justify-between">
        <button onClick={() => setSidebarOpen(true)}>☰ Menu</button>
        <span>KHUSHI BAZAR</span>
      </header>

      <Sidebar isOpen={isSidebarOpen} onClose={() => setSidebarOpen(false)} />
      
      <main className="p-4">
        <h1 className="text-2xl">Welcome</h1>
        <p>Content goes here...</p>
      </main>
    </div>
  );
}

export default App; -->
