import Image from "next/image";

export default function Header() {
  return (
    <header className="fixed top-0 z-50 w-full border-b border-white/10 bg-[#141316]/70 backdrop-blur-xl">
      <div className="mx-auto flex h-16 max-w-md items-center justify-between px-5">

        <div className="flex items-center gap-3">
          <Image
            src="/avatar.png"
            alt="Avatar"
            width={40}
            height={40}
            className="rounded-full border-2 border-lime-400"
          />

          <div>
            <p className="text-xs text-zinc-400">
              LVL 24 Paladin
            </p>
          </div>
        </div>

        <h1 className="absolute left-1/2 -translate-x-1/2 text-4xl font-bold text-yellow-400">
          MoneyQuest
        </h1>

        <div className="text-xs font-semibold text-yellow-400">
          🔥 12 DAY STREAK
        </div>

      </div>
    </header>
  );
}
import Header from "@/components/Header";
import BottomNavigation from "@/components/BottomNavigation";
import StatsChart from "@/components/StatsChart";

export default function ReportsPage() {
  return (
    <>
      <Header />

      <main className="mx-auto max-w-md space-y-6 px-5 pt-24">

        <StatsChart />

        {/* Cards */}

      </main>

      <BottomNavigation />
    </>
  );
}
npm install recharts

"use client";

import {
  AreaChart,
  Area,
  ResponsiveContainer
} from "recharts";

const data = [
  { month: "JAN", value: 25 },
  { month: "FEB", value: 18 },
  { month: "MAR", value: 40 },
  { month: "APR", value: 55 },
  { month: "MAY", value: 70 },
];

export default function StatsChart() {
  return (
    <div className="rounded-3xl bg-[#251E36] p-6">

      <div className="mb-6 flex justify-between">

        <div>
          <h2 className="text-3xl font-bold">
            Monthly Evolution
          </h2>

          <p className="text-zinc-400">
            Net Worth Progress
          </p>
        </div>

        <span className="text-3xl font-bold text-lime-300">
          +14.2%
        </span>

      </div>

      <ResponsiveContainer width="100%" height={250}>
        <AreaChart data={data}>
          <Area
            dataKey="value"
            stroke="#d2bcfa"
            fill="#d2bcfa22"
            strokeWidth={4}
          />
        </AreaChart>
      </ResponsiveContainer>

    </div>
  );
}
