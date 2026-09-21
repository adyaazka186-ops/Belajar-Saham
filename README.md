
Action: view_bulk_cap({"paths":["/app/design_guidelines.json","/app/backend/server.py","/app/backend/.env","/app/frontend/.env","/app/frontend/package.json","/app/backend/requirements.txt","/app/frontend/src/App.js","/app/frontend/src/App.css","/app/frontend/src/index.css","/app/frontend/tailwind.config.js"]})
Observation: ===FILE: /app/design_guidelines.json
[Showing lines 1-123 of 123 total] /app/design_guidelines.json:
1|{
2|  "project_title": "Finosofi - Edukasi Pasar Saham & Filosofi Investasi Jangka Panjang",
3|  "app_type": "educational_blog_and_ai_assistant",
4|  "theme": {
5|    "mode": "dark",
6|    "aesthetic": "Dark Elegant Finance & Stoic Wisdom",
7|    "inspiration": "Bloomberg Terminal precision crossed with Financial Times editorial depth and Stoic philosophy library aesthetic"
8|  },
9|  "responsive": {
10|    "breakpoint": "mobile-first (sm: 640px, md: 768px, lg: 1024px, xl: 1280px)",
11|    "layout": "Grid layouts use grid-cols-1 on mobile, scaling to md:grid-cols-2 and lg:grid-cols-3 or lg:grid-cols-12 for Bento box structures. Navigation transforms to mobile sheet/drawer under 768px. Floating AI Chatbot widget operates as a compact bottom bar/fab on mobile expanding into full screen modal or bottom sheet.",
12|    "typography": "Mobile-first scaling with rem units. Hero H1: text-3xl sm:text-5xl lg:text-6xl; Section H2: text-2xl sm:text-3xl lg:text-4xl; Body: text-sm sm:text-base (minimum 14px on mobile to avoid automatic browser zoom).",
13|    "overflow_guard": "All containers wrapped with w-full max-w-full overflow-x-hidden. Tables and data tickers use horizontally scrollable containers with custom dark scrollbar.",
14|    "tap_targets": "Interactive buttons, chips, and nav items have minimum height of 44px (p-3 / h-11) for fluid touchscreen interaction."
15|  },
16|  "typography": {
17|    "heading_font": "Cormorant Garamond, serif",
18|    "body_font": "Plus Jakarta Sans, sans-serif",
19|    "mono_font": "JetBrains Mono, monospace",
20|    "rules": [
21|      "FORBIDDEN: Do NOT use Inter font for Main or Sub-headings.",
22|      "Headings (H1, H2, H3) use Cormorant Garamond with font-bold or font-semibold and tracking-tight to evoke timeless wisdom and high-end editorial finance.",
23|      "Body text uses Plus Jakarta Sans for extreme readability with leading-relaxed line height.",
24|      "Financial data, market tickers, stock quotes, technical ratios, and code blocks MUST use JetBrains Mono.",
25|      "Overlines & Category Badges MUST be uppercase, text-xs or text-sm, font-mono with wide letter spacing tracking-[0.2em]."
26|    ]
27|  },
28|  "colors": {
29|    "background": {
30|      "main": "#090A0F",
31|      "surface": "#11131F",
32|      "surface_elevated": "#1A1D2C",
33|      "border": "#272C3F"
34|    },
35|    "accents": {
36|      "gold_primary": "#D4AF37",
37|      "gold_hover": "#E5C158",
38|      "gold_muted": "rgba(212, 175, 55, 0.15)",
39|      "emerald_bullish": "#10B981",
40|      "crimson_bearish": "#EF4444",
41|      "amber_risk": "#F59E0B"
42|    },
43|    "text": {
44|      "primary": "#F3F4F6",
45|      "secondary": "#9CA3AF",
46|      "muted": "#6B7280",
47|      "inverse": "#090A0F"
48|    },
49|    "rules": [
50|      "FORBIDDEN: Do NOT use purple gradients (#7351B7 or #8B5CF6) anywhere.",
51|      "Gradients must be strictly subtle black-to-surface or gold accent glows (max 10% opacity).",
52|      "All text colors over dark backgrounds must pass WCAG AA contrast (min 4.5:1 ratio).",
53|      "Interactive states MUST explicitly define text colors on hover/focus (e.g. hover:bg-amber-500/20 hover:text-amber-300)."
54|    ]
55|  },
56|  "categories": [
57|    {
58|      "id": "dasar-pasar-saham",
59|      "title": "Dasar-Dasar Pasar Saham",
60|      "subtitle": "Landasan Mekanisme Pasar & Struktur Modal",
61|      "icon": "TrendingUp",
62|      "description": "Memahami mekanisme bursa efek, cara kerja IPO, valuasi dasar, serta pembentukan harga saham secara fundamental.",
63|      "image": "https://images.unsplash.com/photo-1590283603385-17ffb3a7f29f?crop=entropy&cs=srgb&fm=jpg&ixid=M3w4NTYxOTB8MHwxfHNlYXJjaHxfHxzdG9jayUyMG1hcmtldCUyMHRyYWRpbmclMjBmaW5hbmNlJTIwY2hhcnQlMjBkYXJrfGVufDB8fHx8MTc4OTk2ODQ2MXww&ixlib=rb-4.1.0&q=85"
64|    },
65|    {
66|      "id": "investasi-jangka-panjang",
67|      "title": "Prinsip Investasi Jangka Panjang",
68|      "subtitle": "Compounding, Moat & Nilai Intrinsik",
69|      "icon": "ShieldCheck",
70|      "description": "Filosofi Value Investing ala Warren Buffett & Benjamin Graham: alokasi modal, keunggulan kompetitif, dan dividen.",
71|      "image": "https://images.unsplash.com/photo-1611974789855-9c2a0a7236a3?crop=entropy&cs=srgb&fm=jpg&ixid=M3w4NTYxOTB8MHwxfHNlYXJjaHwyfHxzdG9jayUyMG1hcmtldCUyMHRyYWRpbmclMjBmaW5hbmNlJTIwY2hhcnQlMjBkYXJrfGVufDB8fHx8MTc4OTk2ODQ2MXww&ixlib=rb-4.1.0&q=85"
72|    },
73|    {
74|      "id": "pengembangan-diri",
75|      "title": "Pengembangan Diri & Karakter",
76|      "subtitle": "Kedisiplinan, Keahlian & Alokasi Waktu",
77|      "icon": "UserCheck",
78|      "description": "Membangun modal manusia (human capital), etika kerja, serta kebiasaan membaca & berpikir kritis bagi investor.",
79|      "image": "https://images.unsplash.com/photo-1586165368502-1bad197a6461?crop=entropy&cs=srgb&fm=jpg&ixid=M3w4NjAzOTB8MHwxfHNlYXJjaHwyfHxjaGVzcyUyMHN0cmF0ZWd5JTIwcmlzayUyMGRpc2NpcGxpbmUlMjBkYXJrJTIwYmFja2dyb3VuZHxlbnwwfHx8fDE3ODk5Njg0Njl8MA&ixlib=rb-4.1.0&q=85"
80|    },
81|    {
82|      "id": "filosofi-kehidupan",
83|      "title": "Filosofi Kehidupan",
84|      "subtitle": "Stoikisme, Epistemologi & Kebijaksanaan Finansial",
85|      "icon": "BookOpen",
86|      "description": "Mengintegrasikan pemikiran Stoik, Seneca, & Marcus Aurelius dalam memandang kekayaan, kebahagiaan, dan ketidakpastian.",
87|      "image": "https://images.pexels.com/photos/35730384/pexels-photo-35730384.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
88|    },
89|    {
90|      "id": "analisis-teknikal",
91|      "title": "Analisis Teknikal",
92|      "subtitle": "Struktur Tren, Support-Resistance & Volume",
93|      "icon": "BarChart3",
94|      "description": "Pendekatan rasional membaca dinamika harga, konfirmasi indikator teknis, serta pola pergerakan grafik tanpa ilusi.",
95|      "image": "https://images.unsplash.com/photo-1560221328-12fe60f83ab8?crop=entropy&cs=srgb&fm=jpg&ixid=M3w4NTYxOTB8MHwxfHNlYXJjaHw0fHxzdG9jayUyMG1hcmtldCUyMHRyYWRpbmclMjBmaW5hbmNlJTIwY2hhcnQlMjBkYXJrfGVufDB8fHx8MTc4OTk2ODQ2MXww&ixlib=rb-4.1.0&q=85"
96|    },
97|    {
98|      "id": "psikologi-manajemen-risiko",
99|      "title": "Psikologi & Manajemen Risiko",
100|      "subtitle": "Bias Kognitif, Position Sizing & Ketahanan Mental",
101|      "icon": "Brain",
102|      "description": "Menguasai FOMO, greed, and fear. Strategi pengelolaan risiko modal dan perhitungan Margin of Safety yang disiplin.",
103|      "image": "https://images.unsplash.com/photo-1560174038-da43ac74f01b?crop=entropy&cs=srgb&fm=jpg&ixid=M3w4NjAzOTB8MHwxfHNlYXJjaHwxfHxjaGVzcyUyMHN0cmF0ZWd5JTIwcmlzayUyMGRpc2NpcGxpbmUlMjBkYXJrJTIwYmFja2dyb3VuZHxlbnwwfHx8fDE3ODk5Njg0Njl8MA&ixlib=rb-4.1.0&q=85"
104|    }
105|  ],
106|  "feature_requirements": {
107|    "hero_section": "Financial Terminal Live Header + Hero Headline ('Menguasai Pasar Saham Melalui Kedisiplinan & Filosofi Kehidupan') + Interactive Quick Simulator/Ticker + Call-to-action buttons.",
108|    "category_bento_grid": "6 category items in custom asymmetrical bento cards with dark borders, subtle hover gold outline, read count badges, and direct links.",
109|    "article_listing_page": "Category tabs, Search input with debounced filtering, filter by level (Pemula, Menengah, Mahir), estimated reading time tag, and grid/list view toggle.",
110|    "article_detail_page": "Serif editorial typography, Reading Progress bar fixed at top, Table of Contents drawer/sticky, Interactive Bookmark, Font size customizer (S, M, L), Audio Read Time preview, Key Takeaways summary card, Highlighted quote callout boxes, Related articles recommendation.",
111|    "ai_chatbot_widget": "Floating bottom-right trigger ('Asisten Finansial AI'). Supports interactive Q&A regarding Indonesian market terms, stock analysis, Stoic philosophy quotes, and investment calculations. Include quick question prompts (e.g. 'Apa bedanya PBV dan PER?', 'Bagaimana cara mengatasi FOMO saat saham naik pesat?').",
112|    "market_ticker_tape": "Top bar live simulated ticker (IHSG, BBCA, BBRI, BMRI, TLKM, ASII, UNTR) with real-time green/red price fluctuations to emphasize live finance feel."
113|  },
114|  "instructions_to_main_agent": [
115|    "Build the entire application cleanly in React JavaScript (.js files).",
116|    "Implement the live financial market ticker component at the top of the site.",
117|    "Create realistic mock data for articles covering all 6 categories in formal academic Indonesian.",
118|    "Ensure all buttons, inputs, links, and cards have explicit data-testid attributes (e.g., data-testid='hero-explore-button', data-testid='chatbot-trigger-button', data-testid='article-card-1').",
119|    "Integrate the AI Chatbot widget with smart responsive simulated responses if backend API key is absent, or call the backend `/api/chat` route if configured.",
120|    "Ensure dark elegant design with gold accents (#D4AF37) and zero purple gradients.",
121|    "Verify mobile responsive navigation and touch target padding on all screen sizes."
122|  ]
123|}
[End of file]
===END

===FILE: /app/backend/server.py
[Showing lines 1-89 of 89 total] /app/backend/server.py:
1|from fastapi import FastAPI, APIRouter
2|from dotenv import load_dotenv
3|from starlette.middleware.cors import CORSMiddleware
4|from motor.motor_asyncio import AsyncIOMotorClient
5|import os
6|import logging
7|from pathlib import Path
8|from pydantic import BaseModel, Field, ConfigDict
9|from typing import List
10|import uuid
11|from datetime import datetime, timezone
12|
13|
14|ROOT_DIR = Path(__file__).parent
15|load_dotenv(ROOT_DIR / '.env')
16|
17|# MongoDB connection
18|mongo_url = os.environ['MONGO_URL']
19|client = AsyncIOMotorClient(mongo_url)
20|db = client[os.environ['DB_NAME']]
21|
22|# Create the main app without a prefix
23|app = FastAPI()
24|
25|# Create a router with the /api prefix
26|api_router = APIRouter(prefix="/api")
27|
28|
29|# Define Models
30|class StatusCheck(BaseModel):
31|    model_config = ConfigDict(extra="ignore")  # Ignore MongoDB's _id field
32|    
33|    id: str = Field(default_factory=lambda: str(uuid.uuid4()))
34|    client_name: str
35|    timestamp: datetime = Field(default_factory=lambda: datetime.now(timezone.utc))
36|
37|class StatusCheckCreate(BaseModel):
38|    client_name: str
39|
40|# Add your routes to the router instead of directly to app
41|@api_router.get("/")
42|async def root():
43|    return {"message": "Hello World"}
44|
45|@api_router.post("/status", response_model=StatusCheck)
46|async def create_status_check(input: StatusCheckCreate):
47|    status_dict = input.model_dump()
48|    status_obj = StatusCheck(**status_dict)
49|    
50|    # Convert to dict and serialize datetime to ISO string for MongoDB
51|    doc = status_obj.model_dump()
52|    doc['timestamp'] = doc['timestamp'].isoformat()
53|    
54|    _ = await db.status_checks.insert_one(doc)
55|    return status_obj
56|
57|@api_router.get("/status", response_model=List[StatusCheck])
58|async def get_status_checks():
59|    # Exclude MongoDB's _id field from the query results
60|    status_checks = await db.status_checks.find({}, {"_id": 0}).to_list(1000)
61|    
62|    # Convert ISO string timestamps back to datetime objects
63|    for check in status_checks:
64|        if isinstance(check['timestamp'], str):
65|            check['timestamp'] = datetime.fromisoformat(check['timestamp'])
66|    
67|    return status_checks
68|
69|# Include the router in the main app
70|app.include_router(api_router)
71|
72|app.add_middleware(
73|    CORSMiddleware,
74|    allow_credentials=True,
75|    allow_origins=os.environ.get('CORS_ORIGINS', '*').split(','),
76|    allow_methods=["*"],
77|    allow_headers=["*"],
78|)
79|
80|# Configure logging
81|logging.basicConfig(
82|    level=logging.INFO,
83|    format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'
84|)
85|logger = logging.getLogger(__name__)
86|
87|@app.on_event("shutdown")
88|async def shutdown_db_client():
89|    client.close()
[End of file]
===END

===FILE: /app/backend/.env
[Showing lines 1-3 of 3 total] /app/backend/.env:
1|MONGO_URL="mongodb://localhost:27017"
2|DB_NAME="test_database"
3|CORS_ORIGINS="*"
[End of file]
===END

===FILE: /app/frontend/.env
[Showing lines 1-3 of 3 total] /app/frontend/.env:
1|REACT_APP_BACKEND_URL=https://risk-psychology.preview.emergentagent.com
2|WDS_SOCKET_PORT=443
3|ENABLE_HEALTH_CHECK=false
[End of file]
===END

===FILE: /app/frontend/package.json
[Showing lines 1-144 of 144 total] /app/frontend/package.json:
1|{
2|  "name": "frontend",
3|  "version": "0.1.0",
4|  "private": true,
5|  "dependencies": {
6|    "@hookform/resolvers": "5.0.1",
7|    "@radix-ui/react-accordion": "1.2.8",
8|    "@radix-ui/react-alert-dialog": "1.1.11",
9|    "@radix-ui/react-aspect-ratio": "1.1.4",
10|    "@radix-ui/react-avatar": "1.1.7",
11|    "@radix-ui/react-checkbox": "1.2.3",
12|    "@radix-ui/react-collapsible": "1.1.8",
13|    "@radix-ui/react-context-menu": "2.2.12",
14|    "@radix-ui/react-dialog": "1.1.11",
15|    "@radix-ui/react-dropdown-menu": "2.1.12",
16|    "@radix-ui/react-hover-card": "1.1.11",
17|    "@radix-ui/react-label": "2.1.4",
18|    "@radix-ui/react-menubar": "1.1.12",
19|    "@radix-ui/react-navigation-menu": "1.2.10",
20|    "@radix-ui/react-popover": "1.1.11",
21|    "@radix-ui/react-progress": "1.1.4",
22|    "@radix-ui/react-radio-group": "1.3.4",
23|    "@radix-ui/react-scroll-area": "1.2.6",
24|    "@radix-ui/react-select": "2.2.2",
25|    "@radix-ui/react-separator": "1.1.4",
26|    "@radix-ui/react-slider": "1.3.2",
27|    "@radix-ui/react-slot": "1.2.0",
28|    "@radix-ui/react-switch": "1.2.2",
29|    "@radix-ui/react-tabs": "1.1.9",
30|    "@radix-ui/react-toast": "1.2.11",
31|    "@radix-ui/react-toggle": "1.1.6",
32|    "@radix-ui/react-toggle-group": "1.1.7",
33|    "@radix-ui/react-tooltip": "1.2.4",
34|    "@tanstack/react-query": "5.56.2",
35|    "axios": "1.18.0",
36|    "class-variance-authority": "0.7.1",
37|    "clsx": "2.1.1",
38|    "cmdk": "1.1.1",
39|    "cra-template": "1.2.0",
40|    "date-fns": "4.1.0",
41|    "dayjs": "1.11.13",
42|    "embla-carousel-react": "8.6.0",
43|    "framer-motion": "11.18.0",
44|    "input-otp": "1.4.2",
45|    "lodash": "4.18.1",
46|    "lucide-react": "0.516.0",
47|    "next-themes": "0.4.6",
48|    "react": "19.0.0",
49|    "react-day-picker": "8.10.1",
50|    "react-dom": "19.0.0",
51|    "react-hook-form": "7.56.2",
52|    "react-resizable-panels": "3.0.1",
53|    "react-router-dom": "7.15.0",
54|    "react-scripts": "5.0.1",
55|    "recharts": "3.6.0",
56|    "sonner": "2.0.3",
57|    "swr": "2.3.8",
58|    "tailwind-merge": "3.2.0",
59|    "tailwindcss-animate": "1.0.7",
60|    "vaul": "1.1.2",
61|    "zod": "3.24.4"
62|  },
63|  "scripts": {
64|    "start": "craco start",
65|    "build": "craco build",
66|    "test": "craco test"
67|  },
68|  "browserslist": {
69|    "production": [
70|      ">0.2%",
71|      "not dead",
72|      "not op_mini all"
73|    ],
74|    "development": [
75|      "last 1 chrome version",
76|      "last 1 firefox version",
77|      "last 1 safari version"
78|    ]
79|  },
80|  "devDependencies": {
81|    "@babel/plugin-proposal-private-property-in-object": "7.21.11",
82|    "@craco/craco": "7.1.0",
83|    "@emergentbase/overlay": "https://assets.emergent.sh/npm/emergentbase-overlay-0.1.29.tgz",
84|    "@emergentbase/visual-edits": "https://assets.emergent.sh/npm/emergentbase-visual-edits-1.0.13.tgz",
85|    "@eslint/js": "9.23.0",
86|    "@types/lodash": "4.17.24",
87|    "autoprefixer": "10.4.20",
88|    "dotenv": "16.4.5",
89|    "eslint": "9.23.0",
90|    "eslint-plugin-import": "2.31.0",
91|    "eslint-plugin-jsx-a11y": "6.10.2",
92|    "eslint-plugin-react": "7.37.4",
93|    "eslint-plugin-react-hooks": "5.2.0",
94|    "globals": "15.15.0",
95|    "postcss": "8.5.10",
96|    "tailwindcss": "3.4.17"
97|  },
98|  "resolutions": {
99|    "react-router": "7.15.1",
100|    "node-forge": "1.4.0",
101|    "fast-uri": "3.1.2",
102|    "flatted": "3.4.2",
103|    "qs": "6.15.2",
104|    "diff": "4.0.4",
105|    "follow-redirects": "1.16.0",
106|    "path-to-regexp": "0.1.13",
107|    "rollup": "2.80.0",
108|    "underscore": "1.13.8",
109|    "@babel/plugin-transform-modules-systemjs": "7.29.4",
110|    "@eslint/plugin-kit": "0.3.4",
111|    "shell-quote": "1.9.0",
112|    "jsonpath": "1.3.0",
113|    "nth-check": "2.0.1",
114|    "serialize-javascript": "7.0.5",
115|    "uuid": "11.1.1",
116|    "@tootallnate/once": "2.0.1",
117|    "webpack-dev-server": "5.2.6",
118|    "resolve-url-loader": "5.0.0",
119|    "**/resolve-url-loader/postcss": "8.5.10",
120|    "**/axios/form-data": "4.0.6",
121|    "**/jsdom/form-data": "3.0.5",
122|    "**/postcss-svgo/svgo": "2.8.1",
123|    "**/webpack-dev-server/ws": "8.21.0",
124|    "**/postcss-load-config/yaml": "2.8.3",
125|    "**/cosmiconfig/yaml": "1.10.3",
126|    "**/cssnano/yaml": "1.10.3",
127|    "**/eslint/js-yaml": "4.3.0",
128|    "**/@eslint/eslintrc/js-yaml": "4.3.0",
129|    "**/svgo/js-yaml": "3.15.0",
130|    "**/@istanbuljs/load-nyc-config/js-yaml": "3.15.0",
131|    "**/css-loader/postcss": "8.5.10",
132|    "**/css-minimizer-webpack-plugin/postcss": "8.5.10",
133|    "**/react-scripts/postcss": "8.5.10",
134|    "**/filelist/minimatch": "5.1.8",
135|    "**/anymatch/picomatch": "2.3.2",
136|    "**/micromatch/picomatch": "2.3.2",
137|    "**/readdirp/picomatch": "2.3.2",
138|    "**/jest-util/picomatch": "2.3.2",
139|    "**/tinyglobby/picomatch": "4.0.4",
140|    "http-proxy-middleware": "2.0.10"
141|  },
142|  "packageManager": "yarn@1.22.22+sha512.a6b2f7906b721bba3d67d4aff083df04dad64c399707841b7acf00f6b133b7ac24255f2652fa22ae3534329dc6180534e98d17432037ff6fd140556e2bb3137e"
143|}
144|
[End of file]
===END

===FILE: /app/backend/requirements.txt
[Showing lines 1-29 of 29 total] /app/backend/requirements.txt:
1|fastapi==0.110.1
2|uvicorn==0.25.0
3|boto3>=1.34.129
4|requests-oauthlib>=2.0.0
5|cryptography>=42.0.8
6|python-dotenv>=1.0.1
7|pymongo==4.6.3
8|pydantic>=2.6.4
9|email-validator>=2.2.0
10|pyjwt>=2.10.1
11|bcrypt==4.1.3
12|passlib>=1.7.4
13|tzdata>=2024.2
14|motor==3.3.1
15|pytest>=8.0.0
16|pytest-xdist>=3.6.0
17|black>=24.1.1
18|isort>=5.13.2
19|flake8>=7.0.0
20|mypy>=1.8.0
21|python-jose>=3.3.0
22|requests>=2.31.0
23|pandas>=2.2.0
24|numpy>=1.26.0
25|python-multipart>=0.0.9
26|jq>=1.6.0
27|typer>=0.9.0
28|emergentintegrations==0.2.0
29|
[End of file]
===END

===FILE: /app/frontend/src/App.js
[Showing lines 1-58 of 58 total] /app/frontend/src/App.js:
1|import { useEffect } from "react";
2|import "@/App.css";
3|import { BrowserRouter, Routes, Route } from "react-router-dom";
4|import axios from "axios";
5|import { HOME } from "@/constants/testIds";
6|
7|const BACKEND_URL = process.env.REACT_APP_BACKEND_URL;
8|const API = `${BACKEND_URL}/api`;
9|
10|const Home = () => {
11|  const helloWorldApi = async () => {
12|    try {
13|      const response = await axios.get(`${API}/`);
14|      console.log(response.data.message);
15|    } catch (e) {
16|      console.error(e, `errored out requesting / api`);
17|    }
18|  };
19|
20|  useEffect(() => {
21|    helloWorldApi();
22|  }, []);
23|
24|  return (
25|    // The marker attribute below lets the platform probe detect the stock splash — remove it with this page
26|    <div data-emergent-splash>
27|      <header className="App-header">
28|        <a
29|          data-testid={HOME.emergentLink}
30|          className="App-link"
31|          href="https://emergent.sh"
32|          target="_blank"
33|          rel="noopener noreferrer"
34|        >
35|          <img src="https://avatars.githubusercontent.com/in/1201222?s=120&u=2686cf91179bbafbc7a71bfbc43004cf9ae1acea&v=4" />
36|        </a>
37|        <p className="mt-5">Building something incredible ~!</p>
38|      </header>
39|    </div>
40|  );
41|};
42|
43|function App() {
44|  return (
45|    <div className="App">
46|      <BrowserRouter>
47|        <Routes>
48|          <Route path="/" element={<Home />}>
49|            <Route index element={<Home />} />
50|          </Route>
51|        </Routes>
52|      </BrowserRouter>
53|    </div>
54|  );
55|}
56|
57|export default App;
58|
[End of file]
===END

===FILE: /app/frontend/src/App.css
[Showing lines 1-35 of 35 total] /app/frontend/src/App.css:
1|.App-logo {
2|    height: 40vmin;
3|    pointer-events: none;
4|}
5|
6|@media (prefers-reduced-motion: no-preference) {
7|    .App-logo {
8|        animation: App-logo-spin infinite 20s linear;
9|    }
10|}
11|
12|.App-header {
13|    background-color: #0f0f10;
14|    min-height: 100vh;
15|    display: flex;
16|    flex-direction: column;
17|    align-items: center;
18|    justify-content: center;
19|    font-size: calc(10px + 2vmin);
20|    color: white;
21|}
22|
23|.App-link {
24|    color: #61dafb;
25|}
26|
27|@keyframes App-logo-spin {
28|    from {
29|        transform: rotate(0deg);
30|    }
31|    to {
32|        transform: rotate(360deg);
33|    }
34|}
35|
[End of file]
===END

===FILE: /app/frontend/src/index.css
[Showing lines 1-116 of 116 total] /app/frontend/src/index.css:
1|@tailwind base;
2|@tailwind components;
3|@tailwind utilities;
4|
5|body {
6|    margin: 0;
7|    font-family:
8|        -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen",
9|        "Ubuntu", "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue",
10|        sans-serif;
11|    -webkit-font-smoothing: antialiased;
12|    -moz-osx-font-smoothing: grayscale;
13|}
14|
15|code {
16|    font-family:
17|        source-code-pro, Menlo, Monaco, Consolas, "Courier New", monospace;
18|}
19|
20|@layer base {
21|    :root {
22|        --background: 0 0% 100%;
23|        --foreground: 0 0% 3.9%;
24|        --card: 0 0% 100%;
25|        --card-foreground: 0 0% 3.9%;
26|        --popover: 0 0% 100%;
27|        --popover-foreground: 0 0% 3.9%;
28|        --primary: 0 0% 9%;
29|        --primary-foreground: 0 0% 98%;
30|        --secondary: 0 0% 96.1%;
31|        --secondary-foreground: 0 0% 9%;
32|        --muted: 0 0% 96.1%;
33|        --muted-foreground: 0 0% 45.1%;
34|        --accent: 0 0% 96.1%;
35|        --accent-foreground: 0 0% 9%;
36|        --destructive: 0 84.2% 60.2%;
37|        --destructive-foreground: 0 0% 98%;
38|        --border: 0 0% 89.8%;
39|        --input: 0 0% 89.8%;
40|        --ring: 0 0% 3.9%;
41|        --chart-1: 12 76% 61%;
42|        --chart-2: 173 58% 39%;
43|        --chart-3: 197 37% 24%;
44|        --chart-4: 43 74% 66%;
45|        --chart-5: 27 87% 67%;
46|        --radius: 0.5rem;
47|    }
48|    .dark {
49|        --background: 0 0% 3.9%;
50|        --foreground: 0 0% 98%;
51|        --card: 0 0% 3.9%;
52|        --card-foreground: 0 0% 98%;
53|        --popover: 0 0% 3.9%;
54|        --popover-foreground: 0 0% 98%;
55|        --primary: 0 0% 98%;
56|        --primary-foreground: 0 0% 9%;
57|        --secondary: 0 0% 14.9%;
58|        --secondary-foreground: 0 0% 98%;
59|        --muted: 0 0% 14.9%;
60|        --muted-foreground: 0 0% 63.9%;
61|        --accent: 0 0% 14.9%;
62|        --accent-foreground: 0 0% 98%;
63|        --destructive: 0 62.8% 30.6%;
64|        --destructive-foreground: 0 0% 98%;
65|        --border: 0 0% 14.9%;
66|        --input: 0 0% 14.9%;
67|        --ring: 0 0% 83.1%;
68|        --chart-1: 220 70% 50%;
69|        --chart-2: 160 60% 45%;
70|        --chart-3: 30 80% 55%;
71|        --chart-4: 280 65% 60%;
72|        --chart-5: 340 75% 55%;
73|    }
74|}
75|
76|@layer base {
77|    * {
78|        @apply border-border;
79|    }
80|    body {
81|        @apply bg-background text-foreground;
82|    }
83|}
84|
85|@layer base {
86|    [data-debug-wrapper="true"] {
87|        display: contents !important;
88|    }
89|
90|    [data-debug-wrapper="true"] > * {
91|        margin-left: inherit;
92|        margin-right: inherit;
93|        margin-top: inherit;
94|        margin-bottom: inherit;
95|        padding-left: inherit;
96|        padding-right: inherit;
97|        padding-top: inherit;
98|        padding-bottom: inherit;
99|        column-gap: inherit;
100|        row-gap: inherit;
101|        gap: inherit;
102|        border-left-width: inherit;
103|        border-right-width: inherit;
104|        border-top-width: inherit;
105|        border-bottom-width: inherit;
106|        border-left-style: inherit;
107|        border-right-style: inherit;
108|        border-top-style: inherit;
109|        border-bottom-style: inherit;
110|        border-left-color: inherit;
111|        border-right-color: inherit;
112|        border-top-color: inherit;
113|        border-bottom-color: inherit;
114|    }
115|}
116|
[End of file]
===END

===FILE: /app/frontend/tailwind.config.js
[Showing lines 1-84 of 84 total] /app/frontend/tailwind.config.js:
1|/** @type {import('tailwindcss').Config} */
2|module.exports = {
3|    // `overline` is a Tailwind utility; without this an app's own eyebrow-label class draws a line above the text.
4|    blocklist: ["overline"],
5|    darkMode: ["class"],
6|    content: [
7|    "./src/**/*.{js,jsx,ts,tsx}",
8|    "./public/index.html"
9|  ],
10|  theme: {
11|    extend: {
12|      borderRadius: {
13|        lg: 'var(--radius)',
14|        md: 'calc(var(--radius) - 2px)',
15|        sm: 'calc(var(--radius) - 4px)'
16|      },
17|      colors: {
18|        background: 'hsl(var(--background))',
19|        foreground: 'hsl(var(--foreground))',
20|        card: {
21|          DEFAULT: 'hsl(var(--card))',
22|          foreground: 'hsl(var(--card-foreground))'
23|        },
24|        popover: {
25|          DEFAULT: 'hsl(var(--popover))',
26|          foreground: 'hsl(var(--popover-foreground))'
27|        },
28|        primary: {
29|          DEFAULT: 'hsl(var(--primary))',
30|          foreground: 'hsl(var(--primary-foreground))'
31|        },
32|        secondary: {
33|          DEFAULT: 'hsl(var(--secondary))',
34|          foreground: 'hsl(var(--secondary-foreground))'
35|        },
36|        muted: {
37|          DEFAULT: 'hsl(var(--muted))',
38|          foreground: 'hsl(var(--muted-foreground))'
39|        },
40|        accent: {
41|          DEFAULT: 'hsl(var(--accent))',
42|          foreground: 'hsl(var(--accent-foreground))'
43|        },
44|        destructive: {
45|          DEFAULT: 'hsl(var(--destructive))',
46|          foreground: 'hsl(var(--destructive-foreground))'
47|        },
48|        border: 'hsl(var(--border))',
49|        input: 'hsl(var(--input))',
50|        ring: 'hsl(var(--ring))',
51|        chart: {
52|          '1': 'hsl(var(--chart-1))',
53|          '2': 'hsl(var(--chart-2))',
54|          '3': 'hsl(var(--chart-3))',
55|          '4': 'hsl(var(--chart-4))',
56|          '5': 'hsl(var(--chart-5))'
57|        }
58|      },
59|      keyframes: {
60|        'accordion-down': {
61|          from: {
62|            height: '0'
63|          },
64|          to: {
65|            height: 'var(--radix-accordion-content-height)'
66|          }
67|        },
68|        'accordion-up': {
69|          from: {
70|            height: 'var(--radix-accordion-content-height)'
71|          },
72|          to: {
73|            height: '0'
74|          }
75|        }
76|      },
77|      animation: {
78|        'accordion-down': 'accordion-down 0.2s ease-out',
79|        'accordion-up': 'accordion-up 0.2s ease-out'
80|      }
81|    }
82|  },
83|  plugins: [require("tailwindcss-animate")],
84|};
[End of file]
===END
