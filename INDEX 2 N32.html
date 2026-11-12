import React, { useState, useEffect, useMemo } from 'react';
import {
  Users,
  Calendar,
  Clock,
  CheckCircle,
  AlertCircle,
  MapPin,
  Download,
  Plus,
  Edit,
  Trash2,
  Search,
  Eye,
  LogOut,
  Camera,
  Check,
  X,
  Filter,
  Sparkles,
  Quote,
  Megaphone,
  BarChart2,
  ChevronLeft,
  ChevronRight,
  Phone,
  CreditCard,
  UserPlus,
  FileSpreadsheet,
  Stethoscope,
  Briefcase,
  ClipboardList,
  RefreshCw,
  Navigation,
  Video,
  Presentation,
  Building2,
  Radio
} from 'lucide-react';

// ==========================================
// MASTER ENUMS & INITIAL DATA
// ==========================================
const DEFAULT_HRD_PASS = "admin123";

const DIVISIONS = [
  'HRD (Human Resource)',
  'Admin Finance',
  'Staff Office',
  'Marketing',
  'Project Coordinator',
  'Departemen Dokumentasi',
  'Quality Assurance / QA',
  'Social Media Spexa'
];

const INITIAL_EMPLOYEES = [
  {
    id: 'HRD001',
    name: 'Alyza Fakhriyah Ningsih',
    email: 'alyza.fakhriyah@oasis.co.id',
    dept: 'HRD (Human Resource)',
    role: 'HR Manager',
    userRole: 'Admin / HRD',
    password: 'admin123',
    phone: '+62 812-1001-0001',
    bank: 'BCA - 8830192831',
    baseSalary: 14500000,
    allowances: 2500000,
    photo: 'https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?w=150&auto=format&fit=crop&q=80',
    kpiScore: 98
  },
  {
    id: 'DOC001',
    name: 'Clara Maharani',
    email: 'clara.doc@oasis.co.id',
    dept: 'Departemen Dokumentasi',
    role: 'Head of Documentation',
    userRole: 'Employee / Karyawan',
    password: 'doc123',
    phone: '+62 818-5005-0001',
    bank: 'BCA - 110293847',
    baseSalary: 10500000,
    allowances: 1800000,
    photo: 'https://images.unsplash.com/photo-1534528741775-53994a69daeb?w=150&auto=format&fit=crop&q=80',
    kpiScore: 96
  },
  {
    id: 'DOC002',
    name: 'Dandy Pratama',
    email: 'dandy.doc@oasis.co.id',
    dept: 'Departemen Dokumentasi',
    role: 'Lead Videographer',
    userRole: 'Employee / Karyawan',
    password: 'doc123',
    phone: '+62 818-5005-0002',
    bank: 'BNI - 229384710',
    baseSalary: 7200000,
    allowances: 1100000,
    photo: 'https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=150&auto=format&fit=crop&q=80',
    kpiScore: 91
  },
  {
    id: 'MKT001',
    name: 'Dipta Nugraha',
    email: 'dipta.mkt@oasis.co.id',
    dept: 'Marketing',
    role: 'Head Marketing',
    userRole: 'Employee / Karyawan',
    password: 'mkt123',
    phone: '+62 813-3003-0001',
    bank: 'BCA - 772019283',
    baseSalary: 12000000,
    allowances: 2200000,
    photo: 'https://images.unsplash.com/photo-1500648767791-00dcc994a43e?w=150&auto=format&fit=crop&q=80',
    kpiScore: 95
  },
  {
    id: 'QA001',
    name: 'Maritza Vidyatsabita',
    email: 'maritza.qa@oasis.co.id',
    dept: 'Quality Assurance / QA',
    role: 'Lead Layouter',
    userRole: 'Employee / Karyawan',
    password: 'qa123',
    phone: '+62 819-6006-0001',
    bank: 'BCA - 339201928',
    baseSalary: 7500000,
    allowances: 1200000,
    photo: 'https://images.unsplash.com/photo-1544005313-94ddf0286df2?w=150&auto=format&fit=crop&q=80',
    kpiScore: 89
  }
];

const INITIAL_RECORDS = [
  {
    id: 'REC-101',
    empId: 'DOC002',
    empName: 'Dandy Pratama',
    dept: 'Departemen Dokumentasi',
    category: 'Absensi',
    subType: 'Presensi Reguler',
    date: '2026-11-12',
    clockIn: '08:55',
    clockOut: '17:10',
    location: 'Oasis HQ Umbulharjo, Yogyakarta (-7.8105, 110.3850)',
    detail: 'Presensi Harian Regular Office',
    lateMinutes: 0,
    overrideByAdmin: false,
    status: 'Disetujui'
  },
  {
    id: 'REC-102',
    empId: 'QA001',
    empName: 'Maritza Vidyatsabita',
    dept: 'Quality Assurance / QA',
    category: 'Absensi',
    subType: 'Presensi Reguler',
    date: '2026-11-12',
    clockIn: '09:18',
    clockOut: '17:20',
    location: 'Oasis HQ Umbulharjo, Yogyakarta (-7.8105, 110.3850)',
    detail: 'Presensi Harian (Terlambat 18 Menit)',
    lateMinutes: 18,
    overrideByAdmin: false,
    status: 'Disetujui'
  },
  {
    id: 'REC-103',
    empId: 'DOC002',
    empName: 'Dandy Pratama',
    dept: 'Departemen Dokumentasi',
    category: 'Lembur',
    subType: 'Lembur Project',
    date: '2026-11-13',
    clockIn: '17:30',
    clockOut: '20:30',
    location: 'Studio Concept',
    detail: 'Editing Video Campaign Spexa (3 Jam)',
    lateMinutes: 0,
    overrideByAdmin: false,
    status: 'Menunggu Approval'
  },
  {
    id: 'REC-104',
    empId: 'MKT001',
    empName: 'Dipta Nugraha',
    dept: 'Marketing',
    category: 'Sakit',
    subType: 'Izin Sakit (Surat Dokter)',
    date: '2026-11-14',
    clockIn: '-',
    clockOut: '-',
    location: '-',
    detail: 'Demam tinggi & flu berat (Surat Dokter RS Bethesda terlampir)',
    lateMinutes: 0,
    overrideByAdmin: false,
    status: 'Menunggu Approval'
  },
  {
    id: 'REC-105',
    empId: 'DOC001',
    empName: 'Clara Maharani',
    dept: 'Departemen Dokumentasi',
    category: 'Cuti',
    subType: 'Cuti Tahunan',
    date: '2026-11-18',
    clockIn: '-',
    clockOut: '-',
    location: '-',
    detail: 'Keperluan acara keluarga di luar kota (2 Hari: 18-19 Nov 2026)',
    lateMinutes: 0,
    overrideByAdmin: false,
    status: 'Menunggu Approval'
  },
  {
    id: 'REC-106',
    empId: 'QA001',
    empName: 'Maritza Vidyatsabita',
    dept: 'Quality Assurance / QA',
    category: 'Izin',
    subType: 'Izin Half-Day',
    date: '2026-11-15',
    clockIn: '-',
    clockOut: '-',
    location: '-',
    detail: 'Izin setengah hari pagi untuk perpanjangan SIM & dokumen kependudukan',
    lateMinutes: 0,
    overrideByAdmin: false,
    status: 'Menunggu Approval'
  }
];

const INITIAL_ANNOUNCEMENTS = [
  {
    id: 'ANN-01',
    date: '2026-11-12',
    title: 'Townhall Meeting & Evaluasi Kuartal IV 2026',
    priority: 'Penting',
    content: 'Seluruh karyawan diharapkan hadir tepat waktu pada hari Jumat, 15 November 2026 pukul 15:30 WIB di Aula Utama Oasis Creative Indonesia.'
  },
  {
    id: 'ANN-02',
    date: '2026-11-10',
    title: 'Pembaruan Kebijakan Presensi GPS & Toleransi Jam Masuk',
    priority: 'Info Umum',
    content: 'Batas toleransi jam masuk adalah pukul 09:00 WIB. Keterlambatan mulai pukul 09:01 WIB akan terhitung otomatis oleh sistem.'
  }
];

const INITIAL_TASKS = [
  { id: 'TSK-1', title: 'Rekap & Audit Potongan Absensi November', priority: 'Urgent', period: 'Monthly', pic: 'Alyza Fakhriyah', status: 'In Progress' },
  { id: 'TSK-2', title: 'Screening CV Kandidat Video Editor Batch 4', priority: 'Sedang', period: 'Weekly', pic: 'Alyza Fakhriyah', status: 'To-Do' },
  { id: 'TSK-3', title: 'Persiapan Onboarding Karyawan Baru QA', priority: 'Low', period: 'Weekly', pic: 'Staff HRD', status: 'Done' }
];

const INITIAL_CANDIDATES = [
  {
    id: 'CND-01',
    name: 'Rizky Ramadhan',
    position: 'Motion Graphic Designer',
    interviewDate: '2026-11-14',
    interviewScore: 88,
    skillTestScore: 92,
    notes: 'Portofolio sangat kuat di animasi 2D & After Effects.',
    stage: 'Lolos Tahap Selanjutnya'
  },
  {
    id: 'CND-02',
    name: 'Nadia Putri Kusuma',
    position: 'Social Media Specialist',
    interviewDate: '2026-11-15',
    interviewScore: 82,
    skillTestScore: 85,
    notes: 'Komunikatif, paham tren TikTok & Reels.',
    stage: 'Menunggu Evaluasi'
  }
];

const INITIAL_HRD_AGENDAS = [
  {
    id: 'AGD-101',
    date: '2026-11-12',
    startTime: '09:30',
    endTime: '11:00',
    title: 'Koordinasi Mingguan Manajemen & HOD',
    category: 'Koordinasi Internal',
    description: 'Pembahasan target deliverables mingguan seluruh divisi.',
    location: 'Ruang Meeting Utama'
  },
  {
    id: 'AGD-102',
    date: '2026-11-14',
    startTime: '13:30',
    endTime: '15:00',
    title: 'User Interview Kandidat Motion Graphic',
    category: 'Interview & Rekrutmen',
    description: 'Sesi wawancara user bersama Head of Creative.',
    location: 'Ruang HRD 1 / Zoom'
  },
  {
    id: 'AGD-103',
    date: '2026-11-20',
    startTime: '10:00',
    endTime: '12:00',
    title: 'Audit Internal KPI & Payroll',
    category: 'Audit & Compliance',
    description: 'Pemeriksaan kepatuhan potongan absensi dan evaluasi KPI bulanan.',
    location: 'Ruang Direksi'
  }
];

const FIELD_ACTIVITY_TYPES = [
  { id: 'Visit', label: 'Visit Klien', color: 'bg-blue-600', badge: 'bg-blue-100 text-blue-800', hex: '#2563eb' },
  { id: 'Presentasi', label: 'Presentasi', color: 'bg-indigo-600', badge: 'bg-indigo-100 text-indigo-800', hex: '#4f46e5' },
  { id: 'Photoshoot', label: 'Photoshoot', color: 'bg-amber-600', badge: 'bg-amber-100 text-amber-800', hex: '#d97706' },
  { id: 'Videoshoot', label: 'Videoshoot', color: 'bg-rose-600', badge: 'bg-rose-100 text-rose-800', hex: '#e11d48' }
];

const PRESET_YOGYA_LOCATIONS = [
  { name: 'Oasis Creative HQ (Umbulharjo)', lat: -7.8105, lng: 110.3850 },
  { name: 'Kawasan Malioboro & Titik Nol', lat: -7.7926, lng: 110.3658 },
  { name: 'Prawirotaman Creative Hub', lat: -7.8189, lng: 110.3712 },
  { name: 'Hartono / Pakuwon Mall Sleman', lat: -7.7586, lng: 110.3991 },
  { name: 'Candi Prambanan Heritage Venue', lat: -7.7520, lng: 110.4915 }
];

const INITIAL_FIELD_LOGS = [
  {
    id: 'FLD-201',
    empId: 'DOC002',
    empName: 'Dandy Pratama',
    dept: 'Departemen Dokumentasi',
    photo: 'https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=150&auto=format&fit=crop&q=80',
    activityType: 'Videoshoot',
    clientOrVenue: 'Prawirotaman Heritage Resort',
    notes: 'Produksi video profil & drone footage campaign Spexa Q4',
    lat: -7.8189,
    lng: 110.3712,
    date: '2026-11-12',
    time: '09:45',
    status: 'Aktif di Lokasi'
  },
  {
    id: 'FLD-202',
    empId: 'MKT001',
    empName: 'Dipta Nugraha',
    dept: 'Marketing',
    photo: 'https://images.unsplash.com/photo-1500648767791-00dcc994a43e?w=150&auto=format&fit=crop&q=80',
    activityType: 'Presentasi',
    clientOrVenue: 'PT Jogja Digital Nusantara (Sleman)',
    notes: 'Pitching deck annual branding & social media retainer 2027',
    lat: -7.7586,
    lng: 110.3991,
    date: '2026-11-12',
    time: '10:15',
    status: 'Aktif di Lokasi'
  },
  {
    id: 'FLD-203',
    empId: 'DOC001',
    empName: 'Clara Maharani',
    dept: 'Departemen Dokumentasi',
    photo: 'https://images.unsplash.com/photo-1534528741775-53994a69daeb?w=150&auto=format&fit=crop&q=80',
    activityType: 'Photoshoot',
    clientOrVenue: 'Kawasan Malioboro & Titik Nol',
    notes: 'Editorial katalog produk fashion lokal klien Jogja',
    lat: -7.7926,
    lng: 110.3658,
    date: '2026-11-12',
    time: '09:20',
    status: 'Aktif di Lokasi'
  }
];

const DEFAULT_OFFICE_LOCATION = {
  name: 'Oasis Creative HQ (Umbulharjo)',
  address: 'Jl. Glagahsari No. 45, Warungboto, Kec. Umbulharjo, Kota Yogyakarta, DIY 55164',
  lat: -7.8105,
  lng: 110.3850,
  radiusMeters: 250
};

// Kalkulasi jarak presisi (Haversine Formula dalam meter) antara 2 koordinat GPS
function calculateDistanceMeters(lat1, lon1, lat2, lon2) {
  const R = 6371000;
  const toRad = (deg) => (deg * Math.PI) / 180;
  const dLat = toRad(lat2 - lat1);
  const dLon = toRad(lon2 - lon1);
  const a =
    Math.sin(dLat / 2) * Math.sin(dLat / 2) +
    Math.cos(toRad(lat1)) * Math.cos(toRad(lat2)) * Math.sin(dLon / 2) * Math.sin(dLon / 2);
  const c = 2 * Math.atan2(Math.sqrt(a), Math.sqrt(1 - a));
  return Math.round(R * c);
}

const DEFAULT_MOTIVATIONAL_QUOTE = "Setiap langkah kecil yang kamu lakukan hari ini adalah bagian dari karya besar kita bersama. Semangat berkarya!";

// ==========================================
// OFFICIAL OCR OASIS VECTOR LOGO COMPONENT
// ==========================================
function OcrOasisLogo({ className = "h-9" }) {
  return (
    <svg viewBox="0 0 430 110" className={className} fill="none" xmlns="http://www.w3.org/2000/svg">
      <rect x="6" y="18" width="164" height="74" rx="22" fill="white" />
      <text
        x="24"
        y="69"
        fill="#104480"
        fontFamily="'Lexend', 'Inter', sans-serif"
        fontWeight="900"
        fontSize="44"
        letterSpacing="-1"
      >
        OCR
      </text>
      <path d="M148 54L162 68M162 54L148 68" stroke="#104480" strokeWidth="6" strokeLinecap="round" />
      <text
        x="186"
        y="74"
        fill="white"
        fontFamily="'Lexend', 'Inter', sans-serif"
        fontWeight="900"
        fontSize="58"
        letterSpacing="2"
      >
        OASIS
      </text>
    </svg>
  );
}

// Helper untuk klasifikasi pengajuan lama maupun baru
function classifyApprovalCategory(rec) {
  if (rec.category === 'Izin' || rec.category === 'Cuti' || rec.category === 'Sakit' || rec.category === 'Lembur' || rec.category === 'Ganti Jam') {
    return rec.category;
  }
  const combined = `${rec.subType || ''} ${rec.detail || ''}`.toLowerCase();
  if (combined.includes('sakit')) return 'Sakit';
  if (combined.includes('cuti')) return 'Cuti';
  if (combined.includes('lembur')) return 'Lembur';
  if (combined.includes('ganti')) return 'Ganti Jam';
  return 'Izin';
}

export default function App() {
  // Toast Notification State (Pengganti alert() agar rapi dan responsif)
  const [toastMessage, setToastMessage] = useState(null);
  const showToast = (msg, type = 'success') => {
    setToastMessage({ msg, type });
    setTimeout(() => setToastMessage(null), 3600);
  };

  // Persistence states
  const [employees, setEmployees] = useState(() => {
    const saved = localStorage.getItem('oasis_emp_db_v4');
    return saved ? JSON.parse(saved) : INITIAL_EMPLOYEES;
  });

  const [records, setRecords] = useState(() => {
    const saved = localStorage.getItem('oasis_records_db_v4');
    return saved ? JSON.parse(saved) : INITIAL_RECORDS;
  });

  const [announcements, setAnnouncements] = useState(() => {
    const saved = localStorage.getItem('oasis_announcements_db_v4');
    return saved ? JSON.parse(saved) : INITIAL_ANNOUNCEMENTS;
  });

  const [hrdTasks, setHrdTasks] = useState(() => {
    const saved = localStorage.getItem('oasis_hrd_tasks_db_v4');
    return saved ? JSON.parse(saved) : INITIAL_TASKS;
  });

  const [candidates, setCandidates] = useState(() => {
    const saved = localStorage.getItem('oasis_candidates_db_v4');
    return saved ? JSON.parse(saved) : INITIAL_CANDIDATES;
  });

  const [hrdAgendas, setHrdAgendas] = useState(() => {
    const saved = localStorage.getItem('oasis_agendas_db_v4');
    return saved ? JSON.parse(saved) : INITIAL_HRD_AGENDAS;
  });

  const [fieldLogs, setFieldLogs] = useState(() => {
    const saved = localStorage.getItem('oasis_field_logs_v4');
    return saved ? JSON.parse(saved) : INITIAL_FIELD_LOGS;
  });

  const [officeLocation, setOfficeLocation] = useState(() => {
    const saved = localStorage.getItem('oasis_office_location_v4');
    return saved ? JSON.parse(saved) : DEFAULT_OFFICE_LOCATION;
  });

  const [motivationalQuote, setMotivationalQuote] = useState(() => {
    const saved = localStorage.getItem('oasis_motivational_quote_v4');
    return saved ? saved : DEFAULT_MOTIVATIONAL_QUOTE;
  });

  useEffect(() => { localStorage.setItem('oasis_emp_db_v4', JSON.stringify(employees)); }, [employees]);
  useEffect(() => { localStorage.setItem('oasis_records_db_v4', JSON.stringify(records)); }, [records]);
  useEffect(() => { localStorage.setItem('oasis_announcements_db_v4', JSON.stringify(announcements)); }, [announcements]);
  useEffect(() => { localStorage.setItem('oasis_hrd_tasks_db_v4', JSON.stringify(hrdTasks)); }, [hrdTasks]);
  useEffect(() => { localStorage.setItem('oasis_candidates_db_v4', JSON.stringify(candidates)); }, [candidates]);
  useEffect(() => { localStorage.setItem('oasis_agendas_db_v4', JSON.stringify(hrdAgendas)); }, [hrdAgendas]);
  useEffect(() => { localStorage.setItem('oasis_field_logs_v4', JSON.stringify(fieldLogs)); }, [fieldLogs]);
  useEffect(() => { localStorage.setItem('oasis_office_location_v4', JSON.stringify(officeLocation)); }, [officeLocation]);
  useEffect(() => { localStorage.setItem('oasis_motivational_quote_v4', motivationalQuote); }, [motivationalQuote]);

  // Auth State
  const [isAuthenticated, setIsAuthenticated] = useState(false);
  const [activeLoginRole, setActiveLoginRole] = useState('karyawan');
  const [currentUser, setCurrentUser] = useState(null);

  const [loginEmpId, setLoginEmpId] = useState('');
  const [loginEmpPass, setLoginEmpPass] = useState('');
  const [loginHrdId, setLoginHrdId] = useState('');
  const [loginHrdPass, setLoginHrdPass] = useState('');
  const [loginError, setLoginError] = useState('');

  // Clock State
  const [nowTime, setNowTime] = useState(new Date());
  useEffect(() => {
    const timer = setInterval(() => setNowTime(new Date()), 1000);
    return () => clearInterval(timer);
  }, []);

  // ==========================================
  // KARYAWAN PORTAL STATES
  // ==========================================
  const [gpsCoords, setGpsCoords] = useState(() => ({
    lat: officeLocation.lat,
    lng: officeLocation.lng,
    area: officeLocation.name
  }));
  const [selfieVerified, setSelfieVerified] = useState(false);
  const [karyawanFormTab, setKaryawanFormTab] = useState('perizinan');
  const [fieldDutyForm, setFieldDutyForm] = useState({
    activityType: 'Visit',
    clientOrVenue: '',
    notes: ''
  });
  const [iznForm, setIznForm] = useState({
    category: 'Izin',
    type: 'Izin Mendadak',
    date: '',
    reason: ''
  });
  const [lbrForm, setLbrForm] = useState({ date: '', duration: '2', project: '', reason: '' });
  const [gtForm, setGtForm] = useState({ origDate: '', swapDate: '', reason: '' });

  // ==========================================
  // HRD PORTAL STATES
  // ==========================================
  const [hrdTab, setHrdTab] = useState('dashboard');
  const [selectedRadarPinId, setSelectedRadarPinId] = useState(INITIAL_FIELD_LOGS[0].id);
  const [radarActivityFilter, setRadarActivityFilter] = useState('ALL');
  const [approvalStatusFilter, setApprovalStatusFilter] = useState('ALL'); // 'ALL' | 'Menunggu Approval' | 'Disetujui' | 'Ditolak'
  const [attendanceFilterMonth, setAttendanceFilterMonth] = useState('ALL');
  const [attendanceFilterDept, setAttendanceFilterDept] = useState('ALL');

  // Quote Editor Modal
  const [showQuoteModal, setShowQuoteModal] = useState(false);
  const [tempQuote, setTempQuote] = useState('');

  // Office Location Editor States (HRD)
  const [officeForm, setOfficeForm] = useState(officeLocation);
  useEffect(() => {
    setOfficeForm(officeLocation);
  }, [officeLocation]);

  // Employee CRUD Modal
  const [showEmpModal, setShowEmpModal] = useState(false);
  const [editingEmpId, setEditingEmpId] = useState(null);
  const [empSearch, setEmpSearch] = useState('');
  const [empForm, setEmpForm] = useState({
    id: '', name: '', dept: DIVISIONS[0], role: '', phone: '', bank: '', baseSalary: 7000000, allowances: 1000000, password: 'user123', photo: '', kpiScore: 85
  });

  // Confirm Delete State
  const [confirmDeleteEmp, setConfirmDeleteEmp] = useState(null);

  // KPI Filter & Editing
  const [kpiDeptFilter, setKpiDeptFilter] = useState('ALL');
  const [editingKpiId, setEditingKpiId] = useState(null);
  const [tempKpiVal, setTempKpiVal] = useState(90);

  // HRD Task Filters & Modal
  const [taskPriorityFilter, setTaskPriorityFilter] = useState('ALL');
  const [taskPeriodFilter, setTaskPeriodFilter] = useState('ALL');
  const [newTaskForm, setNewTaskForm] = useState({ title: '', priority: 'Urgent', period: 'Weekly', pic: 'Alyza Fakhriyah' });

  // Candidate Recruitment Modal
  const [showCandModal, setShowCandModal] = useState(false);
  const [candForm, setCandForm] = useState({ name: '', position: '', interviewDate: '', interviewScore: 80, skillTestScore: 80, notes: '' });

  // Announcement Form
  const [annForm, setAnnForm] = useState({ title: '', priority: 'Penting', content: '' });

  // Attendance Override Modal
  const [overrideTarget, setOverrideTarget] = useState(null);
  const [overrideClockIn, setOverrideClockIn] = useState('08:55');
  const [overrideClockOut, setOverrideClockOut] = useState('17:00');

  // Payroll Selected Employee
  const [payrollEmpId, setPayrollEmpId] = useState(INITIAL_EMPLOYEES[1].id);
  const [showSlipModal, setShowSlipModal] = useState(false);

  // HRD Interactive Calendar States
  const [calMonth, setCalMonth] = useState(new Date(2026, 10, 1)); // November 2026
  const [filterAgendaDate, setFilterAgendaDate] = useState('');
  const [filterAgendaTime, setFilterAgendaTime] = useState('');
  const [filterAgendaQuery, setFilterAgendaQuery] = useState('');
  const [showAgendaModal, setShowAgendaModal] = useState(false);
  const [editingAgenda, setEditingAgenda] = useState(null);
  const [agendaForm, setAgendaForm] = useState({
    date: '2026-11-12', startTime: '09:00', endTime: '10:30', title: '', category: 'Meeting Internal', description: '', location: 'Ruang Meeting HRD 1'
  });

  // ==========================================
  // AUTHENTICATION HANDLERS
  // ==========================================
  const handleLogin = (e) => {
    e.preventDefault();
    setLoginError('');

    if (activeLoginRole === 'karyawan') {
      const user = employees.find(
        emp => emp.id.toLowerCase() === loginEmpId.trim().toLowerCase()
      );
      if (!user) {
        setLoginError('ID Karyawan tidak terdaftar di database HRIS Oasis!');
        return;
      }
      if (loginEmpPass !== user.password) {
        setLoginError('Password Karyawan salah! Hubungi HRD jika lupa.');
        return;
      }
      setCurrentUser({ ...user, isHrdAdmin: false });
      setIsAuthenticated(true);
      showToast(`Selamat datang kembali, ${user.name}!`);
    } else {
      const hrdUser = employees.find(
        emp => emp.id.toLowerCase() === loginHrdId.trim().toLowerCase() && emp.userRole.includes('Admin')
      );

      if ((hrdUser && loginHrdPass === hrdUser.password) || (loginHrdId.trim().toUpperCase() === 'HRD001' && loginHrdPass === DEFAULT_HRD_PASS)) {
        setCurrentUser({
          id: hrdUser ? hrdUser.id : 'HRD001',
          name: hrdUser ? hrdUser.name : 'HRD Management',
          isHrdAdmin: true,
          photo: hrdUser ? hrdUser.photo : 'https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?w=150&auto=format&fit=crop&q=80'
        });
        setIsAuthenticated(true);
        showToast('Akses Master HRD & Manajemen aktif.');
      } else {
        setLoginError('ID HRD atau Password HRD tidak valid!');
      }
    }
  };

  const handleLogout = () => {
    setIsAuthenticated(false);
    setCurrentUser(null);
    setLoginEmpId('');
    setLoginEmpPass('');
    setLoginHrdId('');
    setLoginHrdPass('');
    setLoginError('');
  };

  // ==========================================
  // KARYAWAN OPERATIONAL ACTIONS
  // ==========================================
  const dynamicLocationOptions = useMemo(() => {
    const others = PRESET_YOGYA_LOCATIONS.filter(
      loc => !loc.name.toLowerCase().includes('oasis creative hq')
    );
    return [
      { name: officeLocation.name, lat: officeLocation.lat, lng: officeLocation.lng, isOffice: true },
      ...others
    ];
  }, [officeLocation]);

  const currentDistanceFromOffice = useMemo(() => {
    return calculateDistanceMeters(
      gpsCoords.lat,
      gpsCoords.lng,
      officeLocation.lat,
      officeLocation.lng
    );
  }, [gpsCoords, officeLocation]);

  const refreshGps = () => {
    if (navigator.geolocation) {
      navigator.geolocation.getCurrentPosition(
        (pos) => {
          const userLat = Number(pos.coords.latitude.toFixed(6));
          const userLng = Number(pos.coords.longitude.toFixed(6));
          const dist = calculateDistanceMeters(userLat, userLng, officeLocation.lat, officeLocation.lng);
          setGpsCoords({
            lat: userLat,
            lng: userLng,
            area: dist <= officeLocation.radiusMeters
              ? `${officeLocation.name} (Dalam Radius ${dist}m)`
              : `Lokasi GPS Perangkat (${dist}m dari Kantor)`
          });
          showToast('Titik koordinat GPS perangkat berhasil dikunci.');
        },
        () => {
          setGpsCoords({
            lat: officeLocation.lat,
            lng: officeLocation.lng,
            area: officeLocation.name
          });
          showToast(`Koordinat GPS dikunci ke ${officeLocation.name}.`);
        },
        { enableHighAccuracy: true, timeout: 8000 }
      );
    }
  };

  const handleAbsenAction = (type) => {
    if (!selfieVerified) {
      showToast('Wajib melakukan verifikasi foto selfie terlebih dahulu sebelum presensi!', 'error');
      return;
    }
    const todayStr = nowTime.toISOString().split('T')[0];
    const timeStr = `${String(nowTime.getHours()).padStart(2, '0')}:${String(nowTime.getMinutes()).padStart(2, '0')}`;

    const existingIndex = records.findIndex(
      r => r.empId === currentUser.id && r.date === todayStr && r.category === 'Absensi'
    );

    if (type === 'Masuk') {
      if (existingIndex !== -1) {
        showToast('Anda sudah tercatat melakukan Absen Masuk hari ini.', 'error');
        return;
      }
      let lateMins = 0;
      const h = nowTime.getHours();
      const m = nowTime.getMinutes();
      if (h > 9 || (h === 9 && m > 0)) {
        lateMins = (h - 9) * 60 + m;
      }

      const newRec = {
        id: `REC-${Math.floor(100 + Math.random() * 900)}`,
        empId: currentUser.id,
        empName: currentUser.name,
        dept: currentUser.dept,
        category: 'Absensi',
        subType: 'Presensi Reguler',
        date: todayStr,
        clockIn: timeStr,
        clockOut: '--:--',
        location: `${gpsCoords.area} (${gpsCoords.lat}, ${gpsCoords.lng})`,
        detail: lateMins > 0 ? `Presensi Masuk (Terlambat ${lateMins} m)` : 'Presensi Masuk Tepat Waktu',
        lateMinutes: lateMins,
        overrideByAdmin: false,
        status: 'Disetujui'
      };
      setRecords([newRec, ...records]);
      showToast(`Absen Masuk berhasil dicatat pada pukul ${timeStr} WIB!`);
    } else {
      if (existingIndex === -1) {
        showToast('Anda belum melakukan Absen Masuk hari ini!', 'error');
        return;
      }
      const updated = [...records];
      updated[existingIndex] = { ...updated[existingIndex], clockOut: timeStr };
      setRecords(updated);
      showToast(`Absen Pulang berhasil dicatat pada pukul ${timeStr} WIB!`);
    }
  };

  const handleSubmitKaryawanRequest = (e, formCategory) => {
    e.preventDefault();
    const todayStr = nowTime.toISOString().split('T')[0];
    let newRec = {
      id: `REQ-${Math.floor(100 + Math.random() * 900)}`,
      empId: currentUser.id,
      empName: currentUser.name,
      dept: currentUser.dept,
      category: formCategory,
      subType: '',
      date: todayStr,
      clockIn: '-',
      clockOut: '-',
      location: '-',
      detail: '',
      lateMinutes: 0,
      overrideByAdmin: false,
      status: 'Menunggu Approval'
    };

    if (formCategory === 'PerizinanUnified') {
      newRec.category = iznForm.category; // 'Izin' | 'Cuti' | 'Sakit'
      newRec.subType = iznForm.type;
      newRec.date = iznForm.date || todayStr;
      newRec.detail = `${iznForm.type}: ${iznForm.reason}`;
      setIznForm({ category: 'Izin', type: 'Izin Mendadak', date: '', reason: '' });
    } else if (formCategory === 'Lembur') {
      newRec.subType = `${lbrForm.duration} Jam (${lbrForm.project})`;
      newRec.date = lbrForm.date || todayStr;
      newRec.detail = `[${lbrForm.project}] ${lbrForm.duration} Jam - ${lbrForm.reason}`;
      setLbrForm({ date: '', duration: '2', project: '', reason: '' });
    } else if (formCategory === 'Ganti Jam') {
      newRec.subType = `Pengganti tgl ${gtForm.origDate}`;
      newRec.date = gtForm.swapDate || todayStr;
      newRec.detail = `Pengganti tgl ${gtForm.origDate}: ${gtForm.reason}`;
      setGtForm({ origDate: '', swapDate: '', reason: '' });
    }

    setRecords([newRec, ...records]);
    showToast(`Pengajuan ${newRec.category} berhasil terkirim ke Portal HRD!`);
  };

  const handleCheckInFieldDuty = (e) => {
    e.preventDefault();
    if (!fieldDutyForm.clientOrVenue.trim()) {
      showToast('Masukkan nama klien atau lokasi tugas lapangan!', 'error');
      return;
    }
    const todayStr = nowTime.toISOString().split('T')[0];
    const timeStr = `${String(nowTime.getHours()).padStart(2, '0')}:${String(nowTime.getMinutes()).padStart(2, '0')}`;

    const newFieldPin = {
      id: `FLD-${Math.floor(100 + Math.random() * 900)}`,
      empId: currentUser.id,
      empName: currentUser.name,
      dept: currentUser.dept,
      photo: currentUser.photo,
      activityType: fieldDutyForm.activityType,
      clientOrVenue: fieldDutyForm.clientOrVenue,
      notes: fieldDutyForm.notes || `Tugas lapangan ${fieldDutyForm.activityType}`,
      lat: gpsCoords.lat,
      lng: gpsCoords.lng,
      date: todayStr,
      time: timeStr,
      status: 'Aktif di Lokasi'
    };

    setFieldLogs([newFieldPin, ...fieldLogs]);
    setSelectedRadarPinId(newFieldPin.id);
    setFieldDutyForm({ activityType: 'Visit', clientOrVenue: '', notes: '' });
    showToast(`Check-in ${newFieldPin.activityType} di ${newFieldPin.clientOrVenue} terdeteksi di Radar Map HRD!`);
  };

  // ==========================================
  // HRD COMPUTED DATA & SPREADSHEET EXPORT
  // ==========================================
  const filteredAttendanceLogs = useMemo(() => {
    return records.filter(r => {
      if (r.category !== 'Absensi') return false;
      const matchMonth = attendanceFilterMonth === 'ALL' || r.date.startsWith(attendanceFilterMonth);
      const matchDept = attendanceFilterDept === 'ALL' || r.dept === attendanceFilterDept;
      return matchMonth && matchDept;
    });
  }, [records, attendanceFilterMonth, attendanceFilterDept]);

  // Download Spreadsheet Otomatis (.xls untuk Excel rapi berkolom & .csv)
  const handleDownloadAttendanceSpreadsheet = (format = 'xls') => {
    const dataToExport = filteredAttendanceLogs;
    if (dataToExport.length === 0) {
      showToast('Tidak ada data presensi pada filter yang dipilih untuk diunduh.', 'error');
      return;
    }

    const dateStamp = new Date().toISOString().split('T')[0];

    if (format === 'xls') {
      // HTML Table Spreadsheet (.xls) agar kolom otomatis terformat rapi, header berwarna, dan angka tidak rusak di Excel/Google Sheets
      const tableRows = dataToExport
        .map((rec, idx) => {
          const effectiveLate = rec.overrideByAdmin ? 0 : rec.lateMinutes;
          const fine = effectiveLate * 800;
          const statusText = rec.overrideByAdmin
            ? 'Dispensasi HRD'
            : effectiveLate > 0
            ? `Terlambat (${effectiveLate} Menit)`
            : 'Tepat Waktu';

          return `
            <tr>
              <td style="border:1px solid #cbd5e1;padding:6px;text-align:center;">${idx + 1}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;">${rec.id}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;font-weight:bold;">${rec.empId}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;">${rec.empName}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;">${rec.dept}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;text-align:center;">${rec.date}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;text-align:center;">${rec.clockIn}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;text-align:center;">${rec.clockOut}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;">${rec.location}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;text-align:right;">${effectiveLate}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;text-align:right;">${fine}</td>
              <td style="border:1px solid #cbd5e1;padding:6px;font-weight:bold;">${statusText}</td>
            </tr>
          `;
        })
        .join('');

      const excelHtml = `
        <html xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:x="urn:schemas-microsoft-com:office:excel" xmlns="http://www.w3.org/TR/REC-html40">
        <head><meta charset="utf-8" /></head>
        <body>
          <h2 style="font-family:Arial,sans-serif;color:#0b2545;">REKAP PRESENSI KARYAWAN - CV OASIS CREATIVE INDONESIA</h2>
          <p style="font-family:Arial,sans-serif;font-size:12px;color:#475569;">Tanggal Ekspor: ${dateStamp} | Total Baris: ${dataToExport.length}</p>
          <table style="border-collapse:collapse;font-family:Arial,sans-serif;font-size:12px;">
            <thead>
              <tr style="background-color:#0b2545;color:#ffffff;font-weight:bold;">
                <th style="border:1px solid #0b2545;padding:8px;">No</th>
                <th style="border:1px solid #0b2545;padding:8px;">ID Log</th>
                <th style="border:1px solid #0b2545;padding:8px;">ID Karyawan</th>
                <th style="border:1px solid #0b2545;padding:8px;">Nama Karyawan</th>
                <th style="border:1px solid #0b2545;padding:8px;">Divisi / Departemen</th>
                <th style="border:1px solid #0b2545;padding:8px;">Tanggal</th>
                <th style="border:1px solid #0b2545;padding:8px;">Jam Masuk</th>
                <th style="border:1px solid #0b2545;padding:8px;">Jam Pulang</th>
                <th style="border:1px solid #0b2545;padding:8px;">Lokasi GPS</th>
                <th style="border:1px solid #0b2545;padding:8px;">Terlambat (Menit)</th>
                <th style="border:1px solid #0b2545;padding:8px;">Denda Keterlambatan (Rp)</th>
                <th style="border:1px solid #0b2545;padding:8px;">Status Kehadiran</th>
              </tr>
            </thead>
            <tbody>${tableRows}</tbody>
          </table>
        </body>
        </html>
      `;

      const blob = new Blob([excelHtml], { type: 'application/vnd.ms-excel;charset=utf-8;' });
      const url = URL.createObjectURL(blob);
      const link = document.createElement('a');
      link.href = url;
      link.setAttribute('download', `Rekap_Presensi_Oasis_${dateStamp}.xls`);
      document.body.appendChild(link);
      link.click();
      document.body.removeChild(link);
      URL.revokeObjectURL(url);
      showToast('File Excel Spreadsheet (.xls) presensi berhasil diunduh!');
    } else {
      const headers = ['No', 'ID Log', 'ID Karyawan', 'Nama Karyawan', 'Divisi', 'Tanggal', 'Jam Masuk', 'Jam Pulang', 'Lokasi GPS', 'Keterlambatan (Menit)', 'Potongan Denda (Rp)', 'Status'];
      const rows = dataToExport.map((rec, idx) => {
        const effectiveLate = rec.overrideByAdmin ? 0 : rec.lateMinutes;
        const fine = effectiveLate * 800;
        const statusText = rec.overrideByAdmin ? 'Dispensasi HRD' : effectiveLate > 0 ? 'Terlambat' : 'Tepat Waktu';
        return [
          idx + 1,
          rec.id,
          rec.empId,
          `"${rec.empName}"`,
          `"${rec.dept}"`,
          rec.date,
          rec.clockIn,
          rec.clockOut,
          `"${rec.location}"`,
          effectiveLate,
          fine,
          statusText
        ].join(',');
      });

      const csvContent = '\uFEFF' + [headers.join(','), ...rows].join('\n');
      const blob = new Blob([csvContent], { type: 'text/csv;charset=utf-8;' });
      const url = URL.createObjectURL(blob);
      const link = document.createElement('a');
      link.href = url;
      link.setAttribute('download', `Rekap_Presensi_Oasis_${dateStamp}.csv`);
      document.body.appendChild(link);
      link.click();
      document.body.removeChild(link);
      URL.revokeObjectURL(url);
      showToast('File CSV Spreadsheet presensi berhasil diunduh!');
    }
  };

  // Grouping Terpisah untuk Tabel Approval HRD: Izin, Cuti, Sakit, Lembur, Ganti Jam
  const separatedApprovals = useMemo(() => {
    const groups = {
      Izin: [],
      Cuti: [],
      Sakit: [],
      Lembur: [],
      'Ganti Jam': []
    };

    records.forEach(r => {
      if (r.category === 'Absensi') return;
      if (approvalStatusFilter !== 'ALL' && r.status !== approvalStatusFilter) return;

      const normalizedCat = classifyApprovalCategory(r);
      if (groups[normalizedCat]) {
        groups[normalizedCat].push(r);
      } else {
        groups.Izin.push(r);
      }
    });

    return groups;
  }, [records, approvalStatusFilter]);

  const handleUpdateApprovalStatus = (recordId, newStatus) => {
    setRecords(records.map(item => (item.id === recordId ? { ...item, status: newStatus } : item)));
    showToast(`Status pengajuan berhasil diperbarui menjadi "${newStatus}".`);
  };

  const topPerformers = useMemo(() => {
    return [...employees].sort((a, b) => b.kpiScore - a.kpiScore).slice(0, 3);
  }, [employees]);

  const filteredEmployees = useMemo(() => {
    return employees.filter(
      e => e.name.toLowerCase().includes(empSearch.toLowerCase()) || e.id.toLowerCase().includes(empSearch.toLowerCase()) || e.dept.toLowerCase().includes(empSearch.toLowerCase())
    );
  }, [employees, empSearch]);

  const filteredKpiEmployees = useMemo(() => {
    return employees
      .filter(e => kpiDeptFilter === 'ALL' || e.dept === kpiDeptFilter)
      .sort((a, b) => b.kpiScore - a.kpiScore);
  }, [employees, kpiDeptFilter]);

  const filteredTasks = useMemo(() => {
    return hrdTasks.filter(t => {
      const pMatch = taskPriorityFilter === 'ALL' || t.priority === taskPriorityFilter;
      const dMatch = taskPeriodFilter === 'ALL' || t.period === taskPeriodFilter;
      return pMatch && dMatch;
    });
  }, [hrdTasks, taskPriorityFilter, taskPeriodFilter]);

  const filteredAgendas = useMemo(() => {
    return hrdAgendas.filter(ag => {
      const matchDate = !filterAgendaDate || ag.date === filterAgendaDate;
      const matchTime = !filterAgendaTime || ag.startTime.includes(filterAgendaTime);
      const matchQuery =
        !filterAgendaQuery ||
        ag.title.toLowerCase().includes(filterAgendaQuery.toLowerCase()) ||
        ag.category.toLowerCase().includes(filterAgendaQuery.toLowerCase());
      return matchDate && matchTime && matchQuery;
    });
  }, [hrdAgendas, filterAgendaDate, filterAgendaTime, filterAgendaQuery]);

  const calendarDays = useMemo(() => {
    const year = calMonth.getFullYear();
    const month = calMonth.getMonth();
    const firstDay = new Date(year, month, 1).getDay();
    const daysInMonth = new Date(year, month + 1, 0).getDate();
    const cells = [];
    for (let i = 0; i < firstDay; i++) cells.push(null);
    for (let d = 1; d <= daysInMonth; d++) {
      const dateStr = `${year}-${String(month + 1).padStart(2, '0')}-${String(d).padStart(2, '0')}`;
      cells.push({ day: d, dateStr });
    }
    return cells;
  }, [calMonth]);

  const selectedPayrollData = useMemo(() => {
    const emp = employees.find(e => e.id === payrollEmpId) || employees[0];
    const empAbsences = records.filter(r => r.empId === emp.id && r.category === 'Absensi');
    const totalLateMins = empAbsences.reduce((sum, r) => sum + (r.overrideByAdmin ? 0 : r.lateMinutes), 0);
    const lateDeduction = totalLateMins * 800;

    const empLeaves = records.filter(
      r => r.empId === emp.id && r.category !== 'Absensi' && r.status === 'Disetujui'
    );
    const suddenDeduction = empLeaves.filter(l => l.detail.includes('Mendadak')).length * 80000;
    const halfDayDeduction = empLeaves.filter(l => l.detail.includes('Half-Day')).length * 45000;

    const kpiBonus = emp.kpiScore >= 95 ? Math.round(emp.baseSalary * 0.15) : 500000;
    const gross = emp.baseSalary + emp.allowances + kpiBonus;
    const totalDeduction = lateDeduction + suddenDeduction + halfDayDeduction;
    const netSalary = gross - totalDeduction;

    return { emp, totalLateMins, lateDeduction, suddenDeduction, halfDayDeduction, kpiBonus, gross, totalDeduction, netSalary };
  }, [employees, records, payrollEmpId]);

  // ==========================================
  // VIEW 1: PRIVACY-SAFE LOGIN PORTAL
  // ==========================================
  if (!isAuthenticated) {
    return (
      <div className="min-h-screen bg-gradient-to-br from-[#07182e] via-[#0b2545] to-[#104480] flex items-center justify-center p-4 font-sans text-slate-800 antialiased">
        <div className="bg-white/95 backdrop-blur-md rounded-3xl max-w-md w-full p-8 shadow-2xl border border-white/20 text-center relative overflow-hidden space-y-5">
          
          <div className="flex justify-center mb-2">
            <div className="bg-gradient-to-tr from-[#104480] to-[#1D6CB0] p-4 rounded-2xl shadow-xl shadow-[#104480]/30 border border-white/30">
              <OcrOasisLogo className="h-10" />
            </div>
          </div>

          <div>
            <h1 className="text-xl font-extrabold text-[#0b2545] tracking-tight">CV Oasis Creative Indonesia</h1>
            <p className="text-xs text-[#104480] font-semibold">HRIS Enterprise Portal & Operations System</p>
          </div>

          <div className="bg-sky-50/80 border border-sky-200/80 rounded-2xl p-3.5 text-xs text-[#104480] italic font-medium leading-relaxed shadow-sm">
            "{motivationalQuote}"
          </div>

          <div className="flex bg-slate-100 p-1.5 rounded-2xl text-xs font-semibold">
            <button
              type="button"
              onClick={() => { setActiveLoginRole('karyawan'); setLoginError(''); }}
              className={`flex-1 py-2.5 rounded-xl transition-all duration-200 ${activeLoginRole === 'karyawan' ? 'bg-[#0b2545] text-white shadow-md' : 'text-slate-600 hover:text-[#0b2545]'}`}
            >
              Portal Karyawan
            </button>
            <button
              type="button"
              onClick={() => { setActiveLoginRole('hrd'); setLoginError(''); }}
              className={`flex-1 py-2.5 rounded-xl transition-all duration-200 ${activeLoginRole === 'hrd' ? 'bg-[#0b2545] text-white shadow-md' : 'text-slate-600 hover:text-[#0b2545]'}`}
            >
              HRD & Manajemen
            </button>
          </div>

          {loginError && (
            <div className="p-3 bg-rose-50 border border-rose-200 text-rose-700 text-xs rounded-xl font-medium text-left">
              {loginError}
            </div>
          )}

          <form onSubmit={handleLogin} className="space-y-4 text-left">
            {activeLoginRole === 'karyawan' ? (
              <>
                <div>
                  <label className="block text-xs font-bold text-[#0b2545] mb-1">ID Karyawan</label>
                  <input
                    type="text"
                    placeholder="Masukkan ID Karyawan Anda"
                    value={loginEmpId}
                    onChange={(e) => setLoginEmpId(e.target.value)}
                    className="w-full px-4 py-2.5 text-xs rounded-xl border border-slate-300 focus:outline-none focus:ring-2 focus:ring-[#104480] focus:border-[#104480] transition"
                    required
                  />
                </div>
                <div>
                  <label className="block text-xs font-bold text-[#0b2545] mb-1">Password</label>
                  <input
                    type="password"
                    placeholder="Masukkan Password"
                    value={loginEmpPass}
                    onChange={(e) => setLoginEmpPass(e.target.value)}
                    className="w-full px-4 py-2.5 text-xs rounded-xl border border-slate-300 focus:outline-none focus:ring-2 focus:ring-[#104480] focus:border-[#104480] transition"
                    required
                  />
                </div>
              </>
            ) : (
              <>
                <div>
                  <label className="block text-xs font-bold text-[#0b2545] mb-1">ID HRD / Manajemen</label>
                  <input
                    type="text"
                    placeholder="Masukkan ID HRD"
                    value={loginHrdId}
                    onChange={(e) => setLoginHrdId(e.target.value)}
                    className="w-full px-4 py-2.5 text-xs rounded-xl border border-slate-300 focus:outline-none focus:ring-2 focus:ring-[#104480] focus:border-[#104480] transition"
                    required
                  />
                </div>
                <div>
                  <label className="block text-xs font-bold text-[#0b2545] mb-1">Password HRD</label>
                  <input
                    type="password"
                    placeholder="Masukkan Password HRD"
                    value={loginHrdPass}
                    onChange={(e) => setLoginHrdPass(e.target.value)}
                    className="w-full px-4 py-2.5 text-xs rounded-xl border border-slate-300 focus:outline-none focus:ring-2 focus:ring-[#104480] focus:border-[#104480] transition"
                    required
                  />
                </div>
              </>
            )}

            <button
              type="submit"
              className="w-full mt-4 bg-gradient-to-r from-[#0b2545] via-[#104480] to-[#1D6CB0] hover:opacity-95 text-white font-bold py-3.5 rounded-xl shadow-lg shadow-[#104480]/20 transition-all text-xs uppercase tracking-wider"
            >
              Masuk ke Portal System
            </button>
          </form>

        </div>
      </div>
    );
  }

  // ==========================================
  // VIEW 2: AUTHENTICATED APPLICATION SHELL
  // ==========================================
  return (
    <div className="min-h-screen bg-[#f4f7fb] flex flex-col font-sans text-slate-800 antialiased">
      
      {/* Toast Notification Banner */}
      {toastMessage && (
        <div className={`fixed bottom-5 right-5 z-50 px-4 py-3 rounded-2xl shadow-2xl border text-xs font-bold flex items-center gap-2.5 transition-all ${
          toastMessage.type === 'error'
            ? 'bg-rose-600 text-white border-rose-500'
            : 'bg-[#0b2545] text-white border-sky-400'
        }`}>
          {toastMessage.type === 'error' ? <AlertCircle className="w-4 h-4 text-rose-200" /> : <CheckCircle className="w-4 h-4 text-sky-300" />}
          <span>{toastMessage.msg}</span>
        </div>
      )}

      {/* Oasis Corporate Blue Top Header */}
      <header className="bg-gradient-to-r from-[#07182e] via-[#0b2545] to-[#104480] text-white border-b-4 border-[#38bdf8] shadow-lg sticky top-0 z-40">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 py-3 flex justify-between items-center">
          <div className="flex items-center gap-3">
            <OcrOasisLogo className="h-8" />
            <div className="hidden sm:block border-l border-white/20 pl-3">
              <h1 className="font-extrabold text-sm tracking-wide">CV Oasis Creative Indonesia</h1>
              <p className="text-[10px] text-sky-200 font-medium">
                {currentUser.isHrdAdmin ? 'HRD & Management Master System' : 'Portal Mandiri Karyawan'}
              </p>
            </div>
          </div>

          <div className="flex items-center gap-3">
            <span className="hidden md:inline-block px-3 py-1 rounded-full text-[11px] font-bold bg-sky-400/20 text-sky-200 border border-sky-300/30">
              {currentUser.isHrdAdmin ? 'HRD Master Access' : 'Akses Karyawan'}
            </span>
            <img
              src={currentUser.photo}
              alt={currentUser.name}
              className="w-8 h-8 rounded-full object-cover border-2 border-sky-300"
            />
            <div className="text-right hidden sm:block">
              <div className="text-xs font-bold leading-tight">{currentUser.name}</div>
              <div className="text-[10px] text-sky-200 font-mono">{currentUser.id}</div>
            </div>
            <button
              onClick={handleLogout}
              className="bg-white/10 hover:bg-rose-600 text-white px-3 py-1.5 rounded-xl text-xs font-bold border border-white/20 transition flex items-center gap-1.5"
            >
              <LogOut className="w-3.5 h-3.5" />
              <span>Logout</span>
            </button>
          </div>
        </div>
      </header>

      <main className="flex-1 max-w-7xl w-full mx-auto p-4 sm:p-6">

        {/* =================================================================== */}
        {/* VIEW A: INTERFACE KARYAWAN (ISOLATED SELF-SERVICE + PENGUMUMAN)     */}
        {/* =================================================================== */}
        {!currentUser.isHrdAdmin && (
          <div className="space-y-6">
            
            {/* Welcome & Live Clock Banner */}
            <div className="bg-gradient-to-r from-[#0b2545] via-[#104480] to-[#1D6CB0] text-white p-6 rounded-3xl shadow-xl flex flex-col md:flex-row justify-between items-start md:items-center gap-4">
              <div className="space-y-1">
                <span className="text-[11px] font-bold uppercase tracking-wider text-sky-200">Portal Mandiri Karyawan</span>
                <h2 className="font-extrabold text-2xl">Halo, {currentUser.name}!</h2>
                <p className="text-xs text-sky-100 italic">"{motivationalQuote}"</p>
              </div>
              <div className="bg-[#07182e]/70 backdrop-blur-sm px-5 py-3 rounded-2xl border border-sky-300/30 text-right min-w-[210px]">
                <div className="font-mono font-extrabold text-xl text-sky-300">
                  {nowTime.toLocaleTimeString('id-ID')} WIB
                </div>
                <div className="text-xs text-slate-200">
                  {nowTime.toLocaleDateString('id-ID', { weekday: 'long', day: 'numeric', month: 'long', year: 'numeric' })}
                </div>
              </div>
            </div>

            {/* Live Connected Corporate Announcements Board */}
            <div className="bg-white rounded-2xl p-5 shadow-sm border border-sky-200 space-y-3">
              <div className="flex items-center justify-between border-b border-slate-100 pb-2">
                <h3 className="font-bold text-sm text-[#0b2545] flex items-center gap-2">
                  <Megaphone className="w-4 h-4 text-[#104480]" /> Papan Pengumuman Resmi HRD (Live Update)
                </h3>
                <span className="text-[10px] font-bold bg-sky-100 text-[#104480] px-2.5 py-0.5 rounded-full">
                  Terhubung Real-Time
                </span>
              </div>
              <div className="grid grid-cols-1 md:grid-cols-2 gap-3">
                {announcements.map(ann => (
                  <div key={ann.id} className="p-3.5 rounded-xl bg-sky-50/70 border border-sky-100 space-y-1">
                    <div className="flex justify-between items-center">
                      <span className={`text-[10px] font-bold px-2 py-0.5 rounded-full ${ann.priority === 'Penting' ? 'bg-rose-100 text-rose-700' : 'bg-[#104480] text-white'}`}>
                        {ann.priority}
                      </span>
                      <span className="text-[10px] text-slate-400 font-mono">{ann.date}</span>
                    </div>
                    <h4 className="font-bold text-xs text-[#0b2545]">{ann.title}</h4>
                    <p className="text-xs text-slate-600 leading-relaxed">{ann.content}</p>
                  </div>
                ))}
              </div>
            </div>

            {/* GPS Map & Selfie Presensi Section */}
            <div className="grid grid-cols-1 lg:grid-cols-3 gap-6">
              <div className="lg:col-span-2 bg-white rounded-2xl p-5 shadow-sm border border-slate-200 space-y-4">
                <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-2">
                  <div>
                    <h3 className="font-bold text-sm text-[#0b2545] flex items-center gap-1.5">
                      <MapPin className="w-4 h-4 text-[#104480]" /> Live Google Maps & Verifikasi Titik Koordinat GPS
                    </h3>
                    <p className="text-xs text-slate-500">
                      Kantor Pusat: <strong className="text-[#0b2545]">{officeLocation.name}</strong> — {officeLocation.address}
                    </p>
                  </div>
                  <div className="flex flex-wrap items-center gap-2">
                    <select
                      value={gpsCoords.area}
                      onChange={(e) => {
                        const found = dynamicLocationOptions.find(loc => loc.name === e.target.value);
                        if (found) {
                          setGpsCoords({ lat: found.lat, lng: found.lng, area: found.name });
                          showToast(`Titik peta dipindahkan ke ${found.name}`);
                        }
                      }}
                      className="text-xs border border-sky-200 bg-sky-50 text-[#0b2545] font-bold px-2.5 py-1.5 rounded-xl max-w-[230px]"
                    >
                      {dynamicLocationOptions.map(loc => (
                        <option key={loc.name} value={loc.name}>
                          {loc.isOffice ? `🏢 ${loc.name}` : `📍 ${loc.name}`}
                        </option>
                      ))}
                      {!dynamicLocationOptions.some(l => l.name === gpsCoords.area) && (
                        <option value={gpsCoords.area}>{gpsCoords.area}</option>
                      )}
                    </select>
                    <button
                      onClick={refreshGps}
                      className="bg-[#104480] hover:bg-[#0b2545] text-white text-xs font-bold px-3 py-1.5 rounded-xl flex items-center gap-1.5 shadow-sm"
                    >
                      <Navigation className="w-3.5 h-3.5" /> Kunci GPS Saya
                    </button>
                  </div>
                </div>

                {/* Live Google Maps Embed Frame yang Jelas & Tajam */}
                <div className="rounded-2xl h-64 border-2 border-sky-200 relative overflow-hidden shadow-inner bg-slate-100">
                  <iframe
                    title="Google Maps Karyawan"
                    width="100%"
                    height="100%"
                    style={{ border: 0 }}
                    loading="lazy"
                    referrerPolicy="no-referrer-when-downgrade"
                    src={`https://maps.google.com/maps?q=${gpsCoords.lat},${gpsCoords.lng}&z=17&output=embed`}
                  />
                  {/* Floating Coordinate & Status Badge Overlay */}
                  <div className="absolute bottom-3 left-3 right-3 bg-white/95 backdrop-blur-md px-4 py-2.5 rounded-xl border border-sky-200 shadow-lg flex flex-col sm:flex-row justify-between items-start sm:items-center gap-2">
                    <div className="flex items-center gap-2.5">
                      <span className="w-2.5 h-2.5 rounded-full bg-emerald-500 animate-ping" />
                      <div>
                        <div className="font-bold text-xs text-[#0b2545]">{gpsCoords.area}</div>
                        <div className="font-mono text-[11px] text-[#104480]">
                          Koordinat: {gpsCoords.lat}, {gpsCoords.lng} • Jarak ke Kantor: {currentDistanceFromOffice}m (Batas {officeLocation.radiusMeters}m)
                        </div>
                      </div>
                    </div>
                    <span className={`text-[10px] font-bold px-3 py-1 rounded-full ${
                      currentDistanceFromOffice <= officeLocation.radiusMeters
                        ? 'bg-emerald-100 text-emerald-800'
                        : 'bg-sky-100 text-[#104480]'
                    }`}>
                      {currentDistanceFromOffice <= officeLocation.radiusMeters
                        ? '✓ Dalam Radius Kantor'
                        : 'Tugas Luar / Lapangan'}
                    </span>
                  </div>
                </div>
              </div>

              <div className="bg-white rounded-2xl p-5 shadow-sm border border-slate-200 flex flex-col justify-between space-y-4">
                <div className="space-y-3">
                  <h3 className="font-bold text-sm text-[#0b2545]">Verifikasi Selfie & Aksi Absen</h3>
                  <div className="bg-[#07182e] rounded-2xl p-4 text-center text-white space-y-2.5">
                    <div className="w-16 h-16 rounded-full border-2 border-dashed border-sky-400 mx-auto overflow-hidden flex items-center justify-center">
                      {selfieVerified ? (
                        <img src={currentUser.photo} alt="Selfie" className="w-full h-full object-cover" />
                      ) : (
                        <Camera className="w-7 h-7 text-sky-300" />
                      )}
                    </div>
                    <button
                      type="button"
                      onClick={() => {
                        setSelfieVerified(true);
                        showToast('Verifikasi wajah selfie berhasil!');
                      }}
                      className="bg-[#1D6CB0] hover:bg-sky-500 text-white text-[11px] font-bold px-3.5 py-1 rounded-full transition"
                    >
                      {selfieVerified ? 'Selfie Terverifikasi' : 'Ambil Foto Selfie'}
                    </button>
                  </div>
                </div>

                <div className="space-y-2.5">
                  <button
                    onClick={() => handleAbsenAction('Masuk')}
                    className="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-3 rounded-xl text-xs shadow transition"
                  >
                    Absen Masuk
                  </button>
                  <button
                    onClick={() => handleAbsenAction('Pulang')}
                    className="w-full bg-[#104480] hover:bg-[#0b2545] text-white font-bold py-3 rounded-xl text-xs shadow transition"
                  >
                    Absen Pulang
                  </button>
                </div>
              </div>
            </div>

            {/* MENU BARU: CHECK-IN PERJALANAN DINAS / TUGAS LAPANGAN (VISIT, PRESENTASI, PHOTOSHOOT, VIDEOSHOOT) */}
            <div className="bg-white rounded-2xl p-6 shadow-sm border-2 border-sky-200 space-y-4">
              <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-2 border-b border-slate-100 pb-3">
                <div>
                  <div className="flex items-center gap-2">
                    <span className="px-2.5 py-0.5 rounded-full text-[10px] font-extrabold bg-[#104480] text-white uppercase tracking-wider">
                      Live GPS Tracking
                    </span>
                    <h3 className="font-bold text-sm text-[#0b2545]">Check-in Perjalanan Dinas & Tugas Lapangan</h3>
                  </div>
                  <p className="text-xs text-slate-500 mt-0.5">
                    Pilih aktivitas lapangan (Visit, Presentasi, Photoshoot, Videoshoot). Titik lokasi Anda otomatis muncul di Peta Radar HRD.
                  </p>
                </div>
                <div className="text-[11px] font-mono font-bold text-[#104480] bg-sky-50 px-3 py-1.5 rounded-xl border border-sky-200">
                  Pin Aktif: {gpsCoords.lat}, {gpsCoords.lng}
                </div>
              </div>

              <form onSubmit={handleCheckInFieldDuty} className="space-y-4 text-xs">
                {/* Pilihan Jenis Aktivitas Lapangan */}
                <div>
                  <label className="block font-bold text-[#0b2545] mb-2">1. Pilih Jenis Aktivitas Tugas Lapangan</label>
                  <div className="grid grid-cols-2 sm:grid-cols-4 gap-2.5">
                    {FIELD_ACTIVITY_TYPES.map(act => {
                      const isSelected = fieldDutyForm.activityType === act.id;
                      return (
                        <button
                          key={act.id}
                          type="button"
                          onClick={() => setFieldDutyForm({ ...fieldDutyForm, activityType: act.id })}
                          className={`p-3 rounded-xl border-2 text-left transition flex items-center justify-between ${
                            isSelected
                              ? 'border-[#104480] bg-sky-50 text-[#0b2545] shadow-sm'
                              : 'border-slate-200 bg-white text-slate-600 hover:border-sky-300'
                          }`}
                        >
                          <span className="font-extrabold">{act.label}</span>
                          {isSelected && <CheckCircle className="w-4 h-4 text-[#104480]" />}
                        </button>
                      );
                    })}
                  </div>
                </div>

                <div className="grid grid-cols-1 sm:grid-cols-2 gap-4">
                  <div>
                    <label className="block font-bold text-[#0b2545] mb-1">2. Nama Klien / Venue / Lokasi Tujuan</label>
                    <input
                      type="text"
                      placeholder="Contoh: PT Maju Jaya / Studio Malioboro"
                      value={fieldDutyForm.clientOrVenue}
                      onChange={(e) => setFieldDutyForm({ ...fieldDutyForm, clientOrVenue: e.target.value })}
                      className="w-full p-2.5 border border-slate-300 rounded-xl focus:ring-2 focus:ring-[#104480]"
                      required
                    />
                  </div>
                  <div>
                    <label className="block font-bold text-[#0b2545] mb-1">3. Detail Kegiatan & Deliverables</label>
                    <input
                      type="text"
                      placeholder="Contoh: Presentasi proposal Q1 / Shooting konten produk..."
                      value={fieldDutyForm.notes}
                      onChange={(e) => setFieldDutyForm({ ...fieldDutyForm, notes: e.target.value })}
                      className="w-full p-2.5 border border-slate-300 rounded-xl focus:ring-2 focus:ring-[#104480]"
                      required
                    />
                  </div>
                </div>

                <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3 pt-1">
                  <span className="text-[11px] text-slate-500">
                    Koordinat GPS saat ini (<strong>{gpsCoords.area}</strong>) akan langsung dikirim ke Radar Map HRD.
                  </span>
                  <button
                    type="submit"
                    className="bg-gradient-to-r from-[#0b2545] to-[#104480] hover:opacity-95 text-white font-bold px-5 py-2.5 rounded-xl shadow flex items-center gap-2 transition"
                  >
                    <MapPin className="w-4 h-4 text-sky-300" />
                    <span>Kirim Titik Lokasi ({fieldDutyForm.activityType}) ke HRD</span>
                  </button>
                </div>
              </form>

              {/* Riwayat Perjalanan Dinas Pribadi */}
              {fieldLogs.filter(f => f.empId === currentUser.id).length > 0 && (
                <div className="pt-3 border-t border-slate-100">
                  <div className="text-[11px] font-bold text-[#0b2545] mb-2">Log Check-in Perjalanan Dinas Saya:</div>
                  <div className="grid grid-cols-1 md:grid-cols-2 gap-2.5">
                    {fieldLogs
                      .filter(f => f.empId === currentUser.id)
                      .map(log => (
                        <div key={log.id} className="p-3 rounded-xl bg-sky-50/70 border border-sky-100 flex justify-between items-center text-xs">
                          <div>
                            <span className="font-extrabold text-[#104480]">[{log.activityType}]</span>{' '}
                            <span className="font-bold text-[#0b2545]">{log.clientOrVenue}</span>
                            <div className="text-[11px] text-slate-500">{log.notes}</div>
                          </div>
                          <div className="text-right font-mono text-[10px] text-slate-500">
                            <div>{log.date} • {log.time}</div>
                            <div className="text-emerald-700 font-bold">Terdeteksi HRD</div>
                          </div>
                        </div>
                      ))}
                  </div>
                </div>
              )}
            </div>

            {/* Operational Submission Forms (Terkategorisasi otomatis ke tabel Izin, Cuti, Sakit, Lembur, Ganti Jam di Portal HRD) */}
            <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-5">
              <div className="flex flex-wrap gap-2 border-b border-slate-200 pb-3">
                {[
                  { id: 'perizinan', label: 'Pengajuan Izin / Cuti / Sakit' },
                  { id: 'lembur', label: 'Pengajuan Lembur' },
                  { id: 'gantijam', label: 'Pengajuan Ganti Jam' }
                ].map(t => (
                  <button
                    key={t.id}
                    onClick={() => setKaryawanFormTab(t.id)}
                    className={`px-4 py-2 rounded-xl text-xs font-bold transition ${karyawanFormTab === t.id ? 'bg-[#104480] text-white shadow' : 'bg-slate-100 text-slate-600 hover:bg-slate-200'}`}
                  >
                    {t.label}
                  </button>
                ))}
              </div>

              {karyawanFormTab === 'perizinan' && (
                <form onSubmit={(e) => handleSubmitKaryawanRequest(e, 'PerizinanUnified')} className="space-y-4 text-xs">
                  <div className="grid grid-cols-1 sm:grid-cols-3 gap-4">
                    <div>
                      <label className="block font-bold mb-1">Kategori Pengajuan</label>
                      <select
                        value={iznForm.category}
                        onChange={(e) => {
                          const cat = e.target.value;
                          const defaultType =
                            cat === 'Sakit'
                              ? 'Izin Sakit (Surat Dokter)'
                              : cat === 'Cuti'
                              ? 'Cuti Tahunan'
                              : 'Izin Mendadak';
                          setIznForm({ ...iznForm, category: cat, type: defaultType });
                        }}
                        className="w-full p-2.5 border rounded-xl font-bold text-[#0b2545]"
                      >
                        <option value="Izin">Pengajuan Izin</option>
                        <option value="Cuti">Pengajuan Cuti</option>
                        <option value="Sakit">Pengajuan Sakit</option>
                      </select>
                    </div>
                    <div>
                      <label className="block font-bold mb-1">Sub-Jenis {iznForm.category}</label>
                      <select
                        value={iznForm.type}
                        onChange={(e) => setIznForm({ ...iznForm, type: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                      >
                        {iznForm.category === 'Izin' && (
                          <>
                            <option value="Izin Mendadak">Izin Mendadak (1 Hari)</option>
                            <option value="Izin Half-Day">Izin Half-Day (Setengah Hari)</option>
                            <option value="Izin Keperluan Keluarga">Izin Keperluan Keluarga</option>
                          </>
                        )}
                        {iznForm.category === 'Cuti' && (
                          <>
                            <option value="Cuti Tahunan">Cuti Tahunan</option>
                            <option value="Cuti Menikah / Khusus">Cuti Menikah / Khusus</option>
                            <option value="Cuti Melahirkan">Cuti Melahirkan</option>
                          </>
                        )}
                        {iznForm.category === 'Sakit' && (
                          <>
                            <option value="Izin Sakit (Surat Dokter)">Izin Sakit (Dengan Surat Dokter)</option>
                            <option value="Izin Sakit Tanpa Surat Dokter">Izin Sakit (Tanpa Surat Dokter)</option>
                          </>
                        )}
                      </select>
                    </div>
                    <div>
                      <label className="block font-bold mb-1">Tanggal</label>
                      <input
                        type="date"
                        value={iznForm.date}
                        onChange={(e) => setIznForm({ ...iznForm, date: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                        required
                      />
                    </div>
                  </div>
                  <div>
                    <label className="block font-bold mb-1">Alasan & Keterangan Lengkap</label>
                    <input
                      type="text"
                      placeholder="Tuliskan keterangan lengkap pengajuan..."
                      value={iznForm.reason}
                      onChange={(e) => setIznForm({ ...iznForm, reason: e.target.value })}
                      className="w-full p-2.5 border rounded-xl"
                      required
                    />
                  </div>
                  <button type="submit" className="bg-[#104480] hover:bg-[#0b2545] text-white font-bold px-5 py-2.5 rounded-xl">
                    Kirim Pengajuan {iznForm.category} ke HRD
                  </button>
                </form>
              )}

              {karyawanFormTab === 'lembur' && (
                <form onSubmit={(e) => handleSubmitKaryawanRequest(e, 'Lembur')} className="space-y-4 text-xs">
                  <div className="grid grid-cols-1 sm:grid-cols-3 gap-4">
                    <div>
                      <label className="block font-bold mb-1">Tanggal Lembur</label>
                      <input
                        type="date"
                        value={lbrForm.date}
                        onChange={(e) => setLbrForm({ ...lbrForm, date: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                        required
                      />
                    </div>
                    <div>
                      <label className="block font-bold mb-1">Durasi (Jam)</label>
                      <input
                        type="number"
                        min="1"
                        max="12"
                        value={lbrForm.duration}
                        onChange={(e) => setLbrForm({ ...lbrForm, duration: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                        required
                      />
                    </div>
                    <div>
                      <label className="block font-bold mb-1">Project / Klien</label>
                      <input
                        type="text"
                        placeholder="Nama Project"
                        value={lbrForm.project}
                        onChange={(e) => setLbrForm({ ...lbrForm, project: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                        required
                      />
                    </div>
                  </div>
                  <div>
                    <label className="block font-bold mb-1">Detail Pekerjaan</label>
                    <input
                      type="text"
                      placeholder="Target pekerjaan lembur..."
                      value={lbrForm.reason}
                      onChange={(e) => setLbrForm({ ...lbrForm, reason: e.target.value })}
                      className="w-full p-2.5 border rounded-xl"
                      required
                    />
                  </div>
                  <button type="submit" className="bg-[#104480] hover:bg-[#0b2545] text-white font-bold px-5 py-2.5 rounded-xl">
                    Ajukan Lembur
                  </button>
                </form>
              )}

              {karyawanFormTab === 'gantijam' && (
                <form onSubmit={(e) => handleSubmitKaryawanRequest(e, 'Ganti Jam')} className="space-y-4 text-xs">
                  <div className="grid grid-cols-1 sm:grid-cols-2 gap-4">
                    <div>
                      <label className="block font-bold mb-1">Tanggal yang Diganti</label>
                      <input
                        type="date"
                        value={gtForm.origDate}
                        onChange={(e) => setGtForm({ ...gtForm, origDate: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                        required
                      />
                    </div>
                    <div>
                      <label className="block font-bold mb-1">Tanggal Pelaksanaan Pengganti</label>
                      <input
                        type="date"
                        value={gtForm.swapDate}
                        onChange={(e) => setGtForm({ ...gtForm, swapDate: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                        required
                      />
                    </div>
                  </div>
                  <div>
                    <label className="block font-bold mb-1">Keterangan Ganti Jam</label>
                    <input
                      type="text"
                      placeholder="Alasan penggantian jam kerja..."
                      value={gtForm.reason}
                      onChange={(e) => setGtForm({ ...gtForm, reason: e.target.value })}
                      className="w-full p-2.5 border rounded-xl"
                      required
                    />
                  </div>
                  <button type="submit" className="bg-[#104480] hover:bg-[#0b2545] text-white font-bold px-5 py-2.5 rounded-xl">
                    Ajukan Ganti Jam
                  </button>
                </form>
              )}
            </div>

            {/* Personal History Log */}
            <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-4">
              <h3 className="font-bold text-sm text-[#0b2545]">Riwayat Presensi & Status Pengajuan Saya</h3>
              <div className="overflow-x-auto">
                <table className="w-full text-xs text-left">
                  <thead className="bg-[#0b2545] text-white">
                    <tr>
                      <th className="p-3 rounded-tl-xl">Kategori</th>
                      <th className="p-3">Tanggal</th>
                      <th className="p-3">Waktu / Detail</th>
                      <th className="p-3 rounded-tr-xl">Status HRD</th>
                    </tr>
                  </thead>
                  <tbody className="divide-y divide-slate-100">
                    {records
                      .filter(r => r.empId === currentUser.id)
                      .map(r => (
                        <tr key={r.id} className="hover:bg-slate-50">
                          <td className="p-3 font-bold text-[#104480]">
                            {r.category === 'Absensi' ? 'Absensi' : classifyApprovalCategory(r)}
                          </td>
                          <td className="p-3 font-mono">{r.date}</td>
                          <td className="p-3">
                            {r.category === 'Absensi' ? `${r.clockIn} - ${r.clockOut} (${r.detail})` : r.detail}
                          </td>
                          <td className="p-3">
                            <span className={`px-2.5 py-1 rounded-full text-[10px] font-bold ${
                              r.status === 'Disetujui' ? 'bg-emerald-100 text-emerald-800' :
                              r.status === 'Ditolak' ? 'bg-rose-100 text-rose-800' : 'bg-amber-100 text-amber-800'
                            }`}>
                              {r.status}
                            </span>
                          </td>
                        </tr>
                      ))}
                  </tbody>
                </table>
              </div>
            </div>

          </div>
        )}

        {/* =================================================================== */}
        {/* VIEW B: INTERFACE HRD & MANAJEMEN MASTER (CONFIDENTIAL FULL ACCESS) */}
        {/* =================================================================== */}
        {currentUser.isHrdAdmin && (
          <div className="space-y-6">
            
            {/* Confidential HRD Banner & Quick Action Buttons */}
            <div className="bg-gradient-to-r from-sky-50 to-blue-50 border border-sky-200 rounded-2xl p-4 flex flex-col md:flex-row justify-between items-start md:items-center gap-3 text-[#104480] shadow-sm">
              <div className="flex items-center gap-3">
                <div className="w-10 h-10 rounded-xl bg-[#0b2545] text-white flex items-center justify-center font-bold text-sm shadow">
                  HRD
                </div>
                <div>
                  <h3 className="font-bold text-sm text-[#0b2545]">Mode Akses Master HRD / Manajemen Active</h3>
                  <p className="text-xs text-[#104480]">Kewenangan penuh: Approval terpisah (Izin, Cuti, Sakit), export spreadsheet presensi, KPI, & payroll.</p>
                </div>
              </div>

              <div className="flex flex-wrap items-center gap-2">
                <button
                  onClick={() => handleDownloadAttendanceSpreadsheet('xls')}
                  className="bg-emerald-600 hover:bg-emerald-700 text-white text-xs font-bold px-3.5 py-2 rounded-xl shadow flex items-center gap-1.5 transition"
                >
                  <FileSpreadsheet className="w-3.5 h-3.5" />
                  <span>Download Spreadsheet Absensi</span>
                </button>
                <button
                  onClick={() => {
                    setTempQuote(motivationalQuote);
                    setShowQuoteModal(true);
                  }}
                  className="bg-[#104480] hover:bg-[#1D6CB0] text-white text-xs font-bold px-3.5 py-2 rounded-xl shadow flex items-center gap-1.5 transition"
                >
                  <Quote className="w-3.5 h-3.5" />
                  <span>Edit Quote Depan</span>
                </button>
              </div>
            </div>

            {/* HRD Navigation Bar */}
            <div className="flex border-b border-slate-200 gap-2 overflow-x-auto pb-1">
              {[
                { id: 'dashboard', label: 'Dashboard & Approval Terpisah' },
                { id: 'radar-map', label: `Radar Map Perjalanan Dinas (${fieldLogs.length})` },
                { id: 'lokasi-kantor', label: 'Lokasi Kantor & Geofence Map' },
                { id: 'rekap-absent', label: 'Rekap Presensi & Download Excel' },
                { id: 'kalender-hrd', label: 'Kalender Rapat HRD' },
                { id: 'master-emp', label: 'Master Karyawan' },
                { id: 'kpi', label: 'KPI & Hall of Fame' },
                { id: 'rekrutmen', label: 'Rekrutmen & Interview' },
                { id: 'tasks', label: 'To-Do List HRD' },
                { id: 'pengumuman', label: 'Pengumuman Live' },
                { id: 'payroll', label: 'Rekap Gaji & Denda' },
              ].map(tab => (
                <button
                  key={tab.id}
                  onClick={() => setHrdTab(tab.id)}
                  className={`pb-2.5 px-3.5 font-bold text-xs border-b-2 transition whitespace-nowrap ${hrdTab === tab.id ? 'border-[#104480] text-[#104480]' : 'border-transparent text-slate-500 hover:text-slate-800'}`}
                >
                  {tab.label}
                </button>
              ))}
            </div>

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 1: DASHBOARD & TABEL APPROVAL TERPISAH                */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'dashboard' && (
              <div className="space-y-6">
                
                {/* Top Metrics Summary */}
                <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
                  <div className="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm">
                    <div className="text-xs font-bold text-slate-500">Total Karyawan Terdaftar</div>
                    <div className="text-2xl font-extrabold text-[#0b2545] mt-1">{employees.length}</div>
                    <div className="text-[11px] text-emerald-600 font-semibold mt-1">Aktif dalam Database</div>
                  </div>
                  <div
                    onClick={() => setHrdTab('radar-map')}
                    className="bg-white p-5 rounded-2xl border border-sky-200 shadow-sm cursor-pointer hover:border-[#104480] transition"
                  >
                    <div className="text-xs font-bold text-slate-500 flex items-center justify-between">
                      <span>Karyawan Tugas Lapangan</span>
                      <span className="w-2 h-2 rounded-full bg-emerald-500 animate-ping" />
                    </div>
                    <div className="text-2xl font-extrabold text-[#104480] mt-1">{fieldLogs.length} Titik</div>
                    <div className="text-[11px] text-sky-600 font-semibold mt-1">Klik buka Live Radar Map</div>
                  </div>
                  <div className="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm">
                    <div className="text-xs font-bold text-slate-500">Menunggu Approval HRD</div>
                    <div className="text-2xl font-extrabold text-amber-600 mt-1">
                      {records.filter(r => r.category !== 'Absensi' && r.status === 'Menunggu Approval').length}
                    </div>
                    <div className="text-[11px] text-amber-700 font-semibold mt-1">Izin, Cuti, Sakit & Lembur</div>
                  </div>
                  <div className="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm flex flex-col justify-between">
                    <div>
                      <div className="text-xs font-bold text-slate-500">Ekspor Cepat Presensi</div>
                      <div className="text-xs text-slate-600 mt-1">Unduh rekap presensi & denda siap olah.</div>
                    </div>
                    <button
                      onClick={() => handleDownloadAttendanceSpreadsheet('xls')}
                      className="mt-2 w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-2 px-3 rounded-xl text-xs flex items-center justify-center gap-1.5 transition shadow-sm"
                    >
                      <FileSpreadsheet className="w-3.5 h-3.5" />
                      <span>Download Excel (.xls)</span>
                    </button>
                  </div>
                </div>

                {/* MINI LIVE RADAR PREVIEW DALAM 1 FRAME DI DASHBOARD HRD */}
                <div className="bg-white rounded-2xl p-5 shadow-sm border border-sky-200 space-y-4">
                  <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-2">
                    <div>
                      <h3 className="font-bold text-sm text-[#0b2545] flex items-center gap-2">
                        <Radio className="w-4 h-4 text-emerald-600 animate-pulse" />
                        <span>Live Radar Monitoring Perjalanan Dinas (Semua Titik Karyawan dalam 1 Frame)</span>
                      </h3>
                      <p className="text-xs text-slate-500">Deteksi otomatis karyawan yang melakukan Visit, Presentasi, Photoshoot, dan Videoshoot.</p>
                    </div>
                    <button
                      onClick={() => setHrdTab('radar-map')}
                      className="bg-[#104480] hover:bg-[#0b2545] text-white text-xs font-bold px-3.5 py-2 rounded-xl shadow-sm"
                    >
                      Buka Layar Penuh Radar Map
                    </button>
                  </div>

                  {(() => {
                    const visiblePins = fieldLogs.filter(
                      p => radarActivityFilter === 'ALL' || p.activityType === radarActivityFilter
                    );
                    const activePin = visiblePins.find(p => p.id === selectedRadarPinId) || visiblePins[0];
                    // Normalisasi koordinat area Yogyakarta (-7.73 s/d -7.85 lat, 110.33 s/d 110.51 lng) ke posisi % di dalam 1 frame radar
                    const getPinPosition = (lat, lng) => {
                      const topPct = Math.min(84, Math.max(14, ((-7.73 - lat) / 0.12) * 100));
                      const leftPct = Math.min(88, Math.max(12, ((lng - 110.33) / 0.18) * 100));
                      return { top: `${topPct}%`, left: `${leftPct}%` };
                    };

                    return (
                      <div className="grid grid-cols-1 lg:grid-cols-3 gap-4">
                        {/* 1 Frame Map Terpadu dengan Seluruh Titik Karyawan */}
                        <div className="lg:col-span-2 relative h-80 rounded-2xl overflow-hidden border-2 border-[#104480]/30 bg-[#0b2545] shadow-inner">
                          {/* Background Google Maps Terpusat di Area Tugas */}
                          <iframe
                            title="HRD Unified Fleet Radar Map"
                            width="100%"
                            height="100%"
                            style={{ border: 0, filter: 'contrast(1.05)' }}
                            loading="lazy"
                            src={
                              activePin
                                ? `https://maps.google.com/maps?q=${activePin.lat},${activePin.lng}&z=14&output=embed`
                                : `https://maps.google.com/maps?q=${officeLocation.lat},${officeLocation.lng}&z=14&output=embed`
                            }
                          />

                          {/* Overlay Radar Pins untuk SEMUA Karyawan dalam 1 Frame */}
                          <div className="absolute inset-0 pointer-events-none bg-gradient-to-t from-[#07182e]/50 via-transparent to-[#07182e]/20">
                            {/* Pin Kantor Pusat Oasis (Tersinkronisasi dengan Pengaturan Lokasi Kantor HRD) */}
                            {(() => {
                              const hqPos = getPinPosition(officeLocation.lat, officeLocation.lng);
                              return (
                                <div
                                  style={{ top: hqPos.top, left: hqPos.left }}
                                  className="absolute -translate-x-1/2 -translate-y-1/2 z-10"
                                >
                                  <div className="flex items-center gap-1 px-2.5 py-1 rounded-full bg-emerald-700/95 border-2 border-white text-white text-[10px] font-extrabold shadow-lg">
                                    <Building2 className="w-3.5 h-3.5" />
                                    <span>{officeLocation.name}</span>
                                  </div>
                                </div>
                              );
                            })()}
                            {visiblePins.map(pin => {
                              const pos = getPinPosition(pin.lat, pin.lng);
                              const isFocused = activePin && activePin.id === pin.id;
                              const meta = FIELD_ACTIVITY_TYPES.find(a => a.id === pin.activityType) || FIELD_ACTIVITY_TYPES[0];
                              return (
                                <button
                                  key={pin.id}
                                  type="button"
                                  onClick={() => setSelectedRadarPinId(pin.id)}
                                  style={{ top: pos.top, left: pos.left }}
                                  className={`pointer-events-auto absolute -translate-x-1/2 -translate-y-1/2 transition-all duration-300 group ${
                                    isFocused ? 'z-30 scale-110' : 'z-20 hover:scale-105'
                                  }`}
                                >
                                  <div className={`flex items-center gap-1.5 px-2.5 py-1 rounded-full shadow-xl border-2 text-white text-[10px] font-extrabold ${
                                    isFocused ? 'bg-[#0b2545] border-sky-300 ring-4 ring-sky-400/40' : `${meta.color} border-white`
                                  }`}>
                                    <img src={pin.photo} alt={pin.empName} className="w-5 h-5 rounded-full object-cover border border-white" />
                                    <span>{pin.empName.split(' ')[0]}</span>
                                    <span className="bg-white/25 px-1.5 py-0.2 rounded text-[9px]">{pin.activityType}</span>
                                  </div>
                                  <div className="w-0 h-0 border-l-[6px] border-l-transparent border-r-[6px] border-r-transparent border-t-[8px] border-t-white mx-auto" />
                                </button>
                              );
                            })}
                          </div>

                          {/* Legend Aktivitas di Pojok Kiri Bawah Frame */}
                          <div className="absolute bottom-2.5 left-2.5 bg-white/95 backdrop-blur-md px-3 py-1.5 rounded-xl border border-slate-200 shadow flex flex-wrap gap-2 text-[10px] font-bold">
                            {FIELD_ACTIVITY_TYPES.map(t => (
                              <span key={t.id} className="flex items-center gap-1 text-slate-700">
                                <span className={`w-2 h-2 rounded-full ${t.color}`} /> {t.label}
                              </span>
                            ))}
                          </div>
                        </div>

                        {/* Panel Detail Pin Terpilih & Daftar Semua Karyawan di Lapangan */}
                        <div className="bg-slate-50 rounded-2xl p-3.5 border border-slate-200 flex flex-col justify-between space-y-3">
                          <div className="space-y-2 max-h-56 overflow-y-auto pr-1">
                            <div className="text-[11px] font-extrabold text-[#0b2545] uppercase tracking-wider">
                              Titik Karyawan Terdeteksi ({visiblePins.length})
                            </div>
                            {visiblePins.map(pin => {
                              const isFocused = activePin && activePin.id === pin.id;
                              const meta = FIELD_ACTIVITY_TYPES.find(a => a.id === pin.activityType) || FIELD_ACTIVITY_TYPES[0];
                              return (
                                <div
                                  key={pin.id}
                                  onClick={() => setSelectedRadarPinId(pin.id)}
                                  className={`p-2.5 rounded-xl border cursor-pointer transition flex items-start gap-2.5 ${
                                    isFocused ? 'bg-white border-[#104480] shadow-sm ring-1 ring-[#104480]/30' : 'bg-white/70 border-slate-200 hover:bg-white'
                                  }`}
                                >
                                  <img src={pin.photo} alt={pin.empName} className="w-9 h-9 rounded-full object-cover border border-slate-300" />
                                  <div className="flex-1 min-w-0">
                                    <div className="flex justify-between items-center gap-1">
                                      <span className="font-bold text-xs text-[#0b2545] truncate">{pin.empName}</span>
                                      <span className={`px-2 py-0.5 rounded-full text-[9px] font-extrabold ${meta.badge}`}>
                                        {pin.activityType}
                                      </span>
                                    </div>
                                    <div className="text-[11px] font-semibold text-[#104480] truncate">{pin.clientOrVenue}</div>
                                    <div className="text-[10px] text-slate-500 font-mono">{pin.time} WIB • {pin.lat}, {pin.lng}</div>
                                  </div>
                                </div>
                              );
                            })}
                          </div>

                          {activePin && (
                            <div className="bg-[#0b2545] text-white p-3 rounded-xl text-[11px] space-y-1">
                              <div className="font-bold text-sky-300">Fokus Pin: {activePin.empName} ({activePin.activityType})</div>
                              <div className="text-slate-200">{activePin.notes}</div>
                            </div>
                          )}
                        </div>
                      </div>
                    );
                  })()}
                </div>

                {/* Header Kontrol Panel Approval Terpisah */}
                <div className="bg-white rounded-2xl p-5 shadow-sm border border-slate-200 flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3">
                  <div>
                    <h3 className="font-bold text-base text-[#0b2545]">Panel Approval Pengajuan Karyawan (Tabel Terpisah per Kategori)</h3>
                    <p className="text-xs text-slate-500">Setiap jenis pengajuan (Izin, Cuti, Sakit, Lembur, dan Ganti Jam) ditampilkan pada tabel tersendiri untuk memudahkan audit HRD.</p>
                  </div>

                  {/* Filter Status Global untuk Semua Tabel Approval */}
                  <div className="flex items-center gap-2 text-xs">
                    <span className="font-bold text-slate-600">Status:</span>
                    <select
                      value={approvalStatusFilter}
                      onChange={(e) => setApprovalStatusFilter(e.target.value)}
                      className="border border-slate-300 rounded-xl px-3 py-1.5 font-bold text-[#0b2545] bg-slate-50"
                    >
                      <option value="ALL">Semua Status</option>
                      <option value="Menunggu Approval">Menunggu Approval</option>
                      <option value="Disetujui">Disetujui</option>
                      <option value="Ditolak">Ditolak</option>
                    </select>
                  </div>
                </div>

                {/* 3 TABEL UTAMA YANG DIBEDAKAN SECARA EKSPLISIT: IZIN, CUTI, SAKIT */}
                <div className="space-y-6">
                  
                  {/* TABEL 1: PENGAJUAN IZIN */}
                  <div className="bg-white rounded-2xl shadow-sm border border-indigo-200 overflow-hidden">
                    <div className="bg-gradient-to-r from-indigo-900 to-indigo-700 text-white px-5 py-3.5 flex justify-between items-center">
                      <div className="flex items-center gap-2">
                        <ClipboardList className="w-4 h-4 text-indigo-200" />
                        <h4 className="font-bold text-sm">1. Tabel Pengajuan Izin (Half-Day / Mendadak / Keperluan)</h4>
                      </div>
                      <span className="text-[11px] font-bold bg-white/20 px-2.5 py-0.5 rounded-full">
                        {separatedApprovals.Izin.length} Data
                      </span>
                    </div>
                    <div className="overflow-x-auto">
                      <table className="w-full text-xs text-left">
                        <thead className="bg-indigo-50 text-indigo-950 border-b border-indigo-100">
                          <tr>
                            <th className="p-3">Karyawan</th>
                            <th className="p-3">Divisi</th>
                            <th className="p-3">Jenis Izin</th>
                            <th className="p-3">Tanggal</th>
                            <th className="p-3">Keterangan & Alasan</th>
                            <th className="p-3">Status</th>
                            <th className="p-3 text-center">Aksi HRD</th>
                          </tr>
                        </thead>
                        <tbody className="divide-y divide-slate-100">
                          {separatedApprovals.Izin.length === 0 ? (
                            <tr>
                              <td colSpan="7" className="p-5 text-center text-slate-400">Tidak ada data pengajuan Izin.</td>
                            </tr>
                          ) : (
                            separatedApprovals.Izin.map(r => (
                              <tr key={r.id} className="hover:bg-indigo-50/30">
                                <td className="p-3 font-bold text-[#0b2545]">
                                  {r.empName}
                                  <span className="block text-[10px] font-mono text-slate-400">{r.empId}</span>
                                </td>
                                <td className="p-3 text-slate-600">{r.dept}</td>
                                <td className="p-3">
                                  <span className="px-2.5 py-0.5 rounded-md font-bold text-[10px] bg-indigo-100 text-indigo-800">
                                    {r.subType || 'Izin Reguler'}
                                  </span>
                                </td>
                                <td className="p-3 font-mono">{r.date}</td>
                                <td className="p-3">{r.detail}</td>
                                <td className="p-3">
                                  <span className={`px-2.5 py-1 rounded-full text-[10px] font-bold ${
                                    r.status === 'Disetujui' ? 'bg-emerald-100 text-emerald-800' :
                                    r.status === 'Ditolak' ? 'bg-rose-100 text-rose-800' : 'bg-amber-100 text-amber-800'
                                  }`}>
                                    {r.status}
                                  </span>
                                </td>
                                <td className="p-3 text-center">
                                  {r.status === 'Menunggu Approval' ? (
                                    <div className="flex justify-center gap-1.5">
                                      <button
                                        onClick={() => handleUpdateApprovalStatus(r.id, 'Disetujui')}
                                        className="bg-emerald-600 hover:bg-emerald-700 text-white font-bold px-2.5 py-1 rounded-lg text-[11px]"
                                      >
                                        Setujui
                                      </button>
                                      <button
                                        onClick={() => handleUpdateApprovalStatus(r.id, 'Ditolak')}
                                        className="bg-rose-600 hover:bg-rose-700 text-white font-bold px-2.5 py-1 rounded-lg text-[11px]"
                                      >
                                        Tolak
                                      </button>
                                    </div>
                                  ) : (
                                    <span className="text-slate-400 italic">Selesai</span>
                                  )}
                                </td>
                              </tr>
                            ))
                          )}
                        </tbody>
                      </table>
                    </div>
                  </div>

                  {/* TABEL 2: PENGAJUAN CUTI */}
                  <div className="bg-white rounded-2xl shadow-sm border border-sky-200 overflow-hidden">
                    <div className="bg-gradient-to-r from-[#0b2545] to-[#104480] text-white px-5 py-3.5 flex justify-between items-center">
                      <div className="flex items-center gap-2">
                        <Briefcase className="w-4 h-4 text-sky-300" />
                        <h4 className="font-bold text-sm">2. Tabel Pengajuan Cuti (Cuti Tahunan / Cuti Khusus)</h4>
                      </div>
                      <span className="text-[11px] font-bold bg-white/20 px-2.5 py-0.5 rounded-full">
                        {separatedApprovals.Cuti.length} Data
                      </span>
                    </div>
                    <div className="overflow-x-auto">
                      <table className="w-full text-xs text-left">
                        <thead className="bg-sky-50 text-[#0b2545] border-b border-sky-100">
                          <tr>
                            <th className="p-3">Karyawan</th>
                            <th className="p-3">Divisi</th>
                            <th className="p-3">Kategori Cuti</th>
                            <th className="p-3">Tanggal Mulai</th>
                            <th className="p-3">Keterangan Cuti</th>
                            <th className="p-3">Status</th>
                            <th className="p-3 text-center">Aksi HRD</th>
                          </tr>
                        </thead>
                        <tbody className="divide-y divide-slate-100">
                          {separatedApprovals.Cuti.length === 0 ? (
                            <tr>
                              <td colSpan="7" className="p-5 text-center text-slate-400">Tidak ada data pengajuan Cuti.</td>
                            </tr>
                          ) : (
                            separatedApprovals.Cuti.map(r => (
                              <tr key={r.id} className="hover:bg-sky-50/30">
                                <td className="p-3 font-bold text-[#0b2545]">
                                  {r.empName}
                                  <span className="block text-[10px] font-mono text-slate-400">{r.empId}</span>
                                </td>
                                <td className="p-3 text-slate-600">{r.dept}</td>
                                <td className="p-3">
                                  <span className="px-2.5 py-0.5 rounded-md font-bold text-[10px] bg-sky-100 text-[#104480]">
                                    {r.subType || 'Cuti Tahunan'}
                                  </span>
                                </td>
                                <td className="p-3 font-mono">{r.date}</td>
                                <td className="p-3">{r.detail}</td>
                                <td className="p-3">
                                  <span className={`px-2.5 py-1 rounded-full text-[10px] font-bold ${
                                    r.status === 'Disetujui' ? 'bg-emerald-100 text-emerald-800' :
                                    r.status === 'Ditolak' ? 'bg-rose-100 text-rose-800' : 'bg-amber-100 text-amber-800'
                                  }`}>
                                    {r.status}
                                  </span>
                                </td>
                                <td className="p-3 text-center">
                                  {r.status === 'Menunggu Approval' ? (
                                    <div className="flex justify-center gap-1.5">
                                      <button
                                        onClick={() => handleUpdateApprovalStatus(r.id, 'Disetujui')}
                                        className="bg-emerald-600 hover:bg-emerald-700 text-white font-bold px-2.5 py-1 rounded-lg text-[11px]"
                                      >
                                        Setujui
                                      </button>
                                      <button
                                        onClick={() => handleUpdateApprovalStatus(r.id, 'Ditolak')}
                                        className="bg-rose-600 hover:bg-rose-700 text-white font-bold px-2.5 py-1 rounded-lg text-[11px]"
                                      >
                                        Tolak
                                      </button>
                                    </div>
                                  ) : (
                                    <span className="text-slate-400 italic">Selesai</span>
                                  )}
                                </td>
                              </tr>
                            ))
                          )}
                        </tbody>
                      </table>
                    </div>
                  </div>

                  {/* TABEL 3: PENGAJUAN SAKIT */}
                  <div className="bg-white rounded-2xl shadow-sm border border-rose-200 overflow-hidden">
                    <div className="bg-gradient-to-r from-rose-900 to-rose-700 text-white px-5 py-3.5 flex justify-between items-center">
                      <div className="flex items-center gap-2">
                        <Stethoscope className="w-4 h-4 text-rose-200" />
                        <h4 className="font-bold text-sm">3. Tabel Pengajuan Sakit (Verifikasi Surat Dokter & Kesehatan)</h4>
                      </div>
                      <span className="text-[11px] font-bold bg-white/20 px-2.5 py-0.5 rounded-full">
                        {separatedApprovals.Sakit.length} Data
                      </span>
                    </div>
                    <div className="overflow-x-auto">
                      <table className="w-full text-xs text-left">
                        <thead className="bg-rose-50 text-rose-950 border-b border-rose-100">
                          <tr>
                            <th className="p-3">Karyawan</th>
                            <th className="p-3">Divisi</th>
                            <th className="p-3">Kelengkapan Dokumen</th>
                            <th className="p-3">Tanggal Sakit</th>
                            <th className="p-3">Diagnosa / Keterangan</th>
                            <th className="p-3">Status</th>
                            <th className="p-3 text-center">Aksi HRD</th>
                          </tr>
                        </thead>
                        <tbody className="divide-y divide-slate-100">
                          {separatedApprovals.Sakit.length === 0 ? (
                            <tr>
                              <td colSpan="7" className="p-5 text-center text-slate-400">Tidak ada data pengajuan Sakit.</td>
                            </tr>
                          ) : (
                            separatedApprovals.Sakit.map(r => (
                              <tr key={r.id} className="hover:bg-rose-50/30">
                                <td className="p-3 font-bold text-[#0b2545]">
                                  {r.empName}
                                  <span className="block text-[10px] font-mono text-slate-400">{r.empId}</span>
                                </td>
                                <td className="p-3 text-slate-600">{r.dept}</td>
                                <td className="p-3">
                                  <span className="px-2.5 py-0.5 rounded-md font-bold text-[10px] bg-rose-100 text-rose-800">
                                    {r.subType || 'Izin Sakit'}
                                  </span>
                                </td>
                                <td className="p-3 font-mono">{r.date}</td>
                                <td className="p-3">{r.detail}</td>
                                <td className="p-3">
                                  <span className={`px-2.5 py-1 rounded-full text-[10px] font-bold ${
                                    r.status === 'Disetujui' ? 'bg-emerald-100 text-emerald-800' :
                                    r.status === 'Ditolak' ? 'bg-rose-100 text-rose-800' : 'bg-amber-100 text-amber-800'
                                  }`}>
                                    {r.status}
                                  </span>
                                </td>
                                <td className="p-3 text-center">
                                  {r.status === 'Menunggu Approval' ? (
                                    <div className="flex justify-center gap-1.5">
                                      <button
                                        onClick={() => handleUpdateApprovalStatus(r.id, 'Disetujui')}
                                        className="bg-emerald-600 hover:bg-emerald-700 text-white font-bold px-2.5 py-1 rounded-lg text-[11px]"
                                      >
                                        Setujui
                                      </button>
                                      <button
                                        onClick={() => handleUpdateApprovalStatus(r.id, 'Ditolak')}
                                        className="bg-rose-600 hover:bg-rose-700 text-white font-bold px-2.5 py-1 rounded-lg text-[11px]"
                                      >
                                        Tolak
                                      </button>
                                    </div>
                                  ) : (
                                    <span className="text-slate-400 italic">Selesai</span>
                                  )}
                                </td>
                              </tr>
                            ))
                          )}
                        </tbody>
                      </table>
                    </div>
                  </div>

                  {/* TABEL 4 & 5: PENGAJUAN LEMBUR & GANTI JAM */}
                  <div className="grid grid-cols-1 lg:grid-cols-2 gap-6">
                    {/* Tabel Lembur */}
                    <div className="bg-white rounded-2xl shadow-sm border border-amber-200 overflow-hidden">
                      <div className="bg-gradient-to-r from-amber-800 to-amber-600 text-white px-5 py-3 flex justify-between items-center">
                        <div className="flex items-center gap-2">
                          <Clock className="w-4 h-4 text-amber-200" />
                          <h4 className="font-bold text-xs">4. Tabel Pengajuan Lembur</h4>
                        </div>
                        <span className="text-[10px] font-bold bg-white/20 px-2 py-0.5 rounded-full">
                          {separatedApprovals.Lembur.length} Data
                        </span>
                      </div>
                      <div className="overflow-x-auto">
                        <table className="w-full text-xs text-left">
                          <thead className="bg-amber-50 text-amber-950 border-b border-amber-100">
                            <tr>
                              <th className="p-2.5">Karyawan</th>
                              <th className="p-2.5">Tanggal</th>
                              <th className="p-2.5">Detail Lembur</th>
                              <th className="p-2.5 text-center">Aksi</th>
                            </tr>
                          </thead>
                          <tbody className="divide-y divide-slate-100">
                            {separatedApprovals.Lembur.length === 0 ? (
                              <tr>
                                <td colSpan="4" className="p-4 text-center text-slate-400">Tidak ada pengajuan Lembur.</td>
                              </tr>
                            ) : (
                              separatedApprovals.Lembur.map(r => (
                                <tr key={r.id}>
                                  <td className="p-2.5 font-bold text-[#0b2545]">{r.empName}</td>
                                  <td className="p-2.5 font-mono">{r.date}</td>
                                  <td className="p-2.5">{r.detail}</td>
                                  <td className="p-2.5 text-center">
                                    {r.status === 'Menunggu Approval' ? (
                                      <div className="flex justify-center gap-1">
                                        <button onClick={() => handleUpdateApprovalStatus(r.id, 'Disetujui')} className="bg-emerald-600 text-white px-2 py-1 rounded text-[10px] font-bold">Acc</button>
                                        <button onClick={() => handleUpdateApprovalStatus(r.id, 'Ditolak')} className="bg-rose-600 text-white px-2 py-1 rounded text-[10px] font-bold">Tolak</button>
                                      </div>
                                    ) : (
                                      <span className="text-[10px] font-bold text-slate-500">{r.status}</span>
                                    )}
                                  </td>
                                </tr>
                              ))
                            )}
                          </tbody>
                        </table>
                      </div>
                    </div>

                    {/* Tabel Ganti Jam */}
                    <div className="bg-white rounded-2xl shadow-sm border border-teal-200 overflow-hidden">
                      <div className="bg-gradient-to-r from-teal-800 to-teal-600 text-white px-5 py-3 flex justify-between items-center">
                        <div className="flex items-center gap-2">
                          <RefreshCw className="w-4 h-4 text-teal-200" />
                          <h4 className="font-bold text-xs">5. Tabel Pengajuan Ganti Jam</h4>
                        </div>
                        <span className="text-[10px] font-bold bg-white/20 px-2 py-0.5 rounded-full">
                          {separatedApprovals['Ganti Jam'].length} Data
                        </span>
                      </div>
                      <div className="overflow-x-auto">
                        <table className="w-full text-xs text-left">
                          <thead className="bg-teal-50 text-teal-950 border-b border-teal-100">
                            <tr>
                              <th className="p-2.5">Karyawan</th>
                              <th className="p-2.5">Tanggal</th>
                              <th className="p-2.5">Keterangan</th>
                              <th className="p-2.5 text-center">Aksi</th>
                            </tr>
                          </thead>
                          <tbody className="divide-y divide-slate-100">
                            {separatedApprovals['Ganti Jam'].length === 0 ? (
                              <tr>
                                <td colSpan="4" className="p-4 text-center text-slate-400">Tidak ada pengajuan Ganti Jam.</td>
                              </tr>
                            ) : (
                              separatedApprovals['Ganti Jam'].map(r => (
                                <tr key={r.id}>
                                  <td className="p-2.5 font-bold text-[#0b2545]">{r.empName}</td>
                                  <td className="p-2.5 font-mono">{r.date}</td>
                                  <td className="p-2.5">{r.detail}</td>
                                  <td className="p-2.5 text-center">
                                    {r.status === 'Menunggu Approval' ? (
                                      <div className="flex justify-center gap-1">
                                        <button onClick={() => handleUpdateApprovalStatus(r.id, 'Disetujui')} className="bg-emerald-600 text-white px-2 py-1 rounded text-[10px] font-bold">Acc</button>
                                        <button onClick={() => handleUpdateApprovalStatus(r.id, 'Ditolak')} className="bg-rose-600 text-white px-2 py-1 rounded text-[10px] font-bold">Tolak</button>
                                      </div>
                                    ) : (
                                      <span className="text-[10px] font-bold text-slate-500">{r.status}</span>
                                    )}
                                  </td>
                                </tr>
                              ))
                            )}
                          </tbody>
                        </table>
                      </div>
                    </div>
                  </div>

                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB KHUSUS: LIVE RADAR MAP PERJALANAN DINAS FULL VIEW     */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'radar-map' && (
              <div className="space-y-6">
                <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-5">
                  <div className="flex flex-col md:flex-row justify-between items-start md:items-center gap-4 border-b pb-4">
                    <div>
                      <h3 className="font-bold text-base text-[#0b2545] flex items-center gap-2">
                        <MapPin className="w-5 h-5 text-[#104480]" /> Pusat Pantauan GPS Perjalanan Dinas & Tugas Lapangan
                      </h3>
                      <p className="text-xs text-slate-500">
                        Semua karyawan yang melakukan check-in Visit, Presentasi, Photoshoot, dan Videoshoot ditampilkan secara serentak dalam 1 layar peta.
                      </p>
                    </div>

                    {/* Filter Jenis Aktivitas Lapangan */}
                    <div className="flex flex-wrap gap-1.5 text-xs">
                      <button
                        onClick={() => setRadarActivityFilter('ALL')}
                        className={`px-3 py-1.5 rounded-xl font-bold transition ${
                          radarActivityFilter === 'ALL' ? 'bg-[#0b2545] text-white shadow' : 'bg-slate-100 text-slate-600'
                        }`}
                      >
                        Semua ({fieldLogs.length})
                      </button>
                      {FIELD_ACTIVITY_TYPES.map(act => (
                        <button
                          key={act.id}
                          onClick={() => setRadarActivityFilter(act.id)}
                          className={`px-3 py-1.5 rounded-xl font-bold transition ${
                            radarActivityFilter === act.id ? `${act.color} text-white shadow` : 'bg-slate-100 text-slate-600'
                          }`}
                        >
                          {act.label} ({fieldLogs.filter(f => f.activityType === act.id).length})
                        </button>
                      ))}
                    </div>
                  </div>

                  {(() => {
                    const visiblePins = fieldLogs.filter(
                      p => radarActivityFilter === 'ALL' || p.activityType === radarActivityFilter
                    );
                    const activePin = visiblePins.find(p => p.id === selectedRadarPinId) || visiblePins[0];
                    const getPinPosition = (lat, lng) => {
                      const topPct = Math.min(84, Math.max(14, ((-7.73 - lat) / 0.12) * 100));
                      const leftPct = Math.min(88, Math.max(12, ((lng - 110.33) / 0.18) * 100));
                      return { top: `${topPct}%`, left: `${leftPct}%` };
                    };

                    return (
                      <div className="space-y-5">
                        {/* Unified Full-Width Map Frame */}
                        <div className="relative h-[430px] rounded-3xl overflow-hidden border-2 border-[#104480]/40 shadow-xl bg-[#07182e]">
                          <iframe
                            title="HRD Full Radar Map"
                            width="100%"
                            height="100%"
                            style={{ border: 0 }}
                            loading="lazy"
                            src={
                              activePin
                                ? `https://maps.google.com/maps?q=${activePin.lat},${activePin.lng}&z=15&output=embed`
                                : `https://maps.google.com/maps?q=${officeLocation.lat},${officeLocation.lng}&z=15&output=embed`
                            }
                          />

                          {/* Multi-Employee Pin Overlay */}
                          <div className="absolute inset-0 pointer-events-none bg-gradient-to-t from-[#07182e]/60 via-transparent to-transparent">
                            {/* Titik Kantor Pusat dari Pengaturan HRD */}
                            {(() => {
                              const hqPos = getPinPosition(officeLocation.lat, officeLocation.lng);
                              return (
                                <div
                                  style={{ top: hqPos.top, left: hqPos.left }}
                                  className="absolute -translate-x-1/2 -translate-y-1/2 z-10"
                                >
                                  <div className="flex items-center gap-1.5 px-3 py-1 rounded-2xl bg-emerald-700 border-2 border-white text-white text-[11px] font-extrabold shadow-xl">
                                    <Building2 className="w-4 h-4" />
                                    <span>Kantor: {officeLocation.name}</span>
                                  </div>
                                </div>
                              );
                            })()}
                            {visiblePins.map(pin => {
                              const pos = getPinPosition(pin.lat, pin.lng);
                              const isFocused = activePin && activePin.id === pin.id;
                              const meta = FIELD_ACTIVITY_TYPES.find(a => a.id === pin.activityType) || FIELD_ACTIVITY_TYPES[0];
                              return (
                                <button
                                  key={pin.id}
                                  type="button"
                                  onClick={() => setSelectedRadarPinId(pin.id)}
                                  style={{ top: pos.top, left: pos.left }}
                                  className={`pointer-events-auto absolute -translate-x-1/2 -translate-y-1/2 transition-all duration-300 ${
                                    isFocused ? 'z-30 scale-115' : 'z-20 hover:scale-105'
                                  }`}
                                >
                                  <div className={`flex items-center gap-2 px-3 py-1.5 rounded-2xl shadow-2xl border-2 text-white text-xs font-extrabold ${
                                    isFocused ? 'bg-[#0b2545] border-sky-300 ring-4 ring-sky-400/50' : `${meta.color} border-white`
                                  }`}>
                                    <img src={pin.photo} alt={pin.empName} className="w-6 h-6 rounded-full object-cover border border-white" />
                                    <div className="text-left">
                                      <div className="leading-none">{pin.empName}</div>
                                      <div className="text-[9px] text-sky-200 font-semibold mt-0.5">{pin.activityType} • {pin.time}</div>
                                    </div>
                                  </div>
                                  <div className="w-0 h-0 border-l-[7px] border-l-transparent border-r-[7px] border-r-transparent border-t-[9px] border-t-white mx-auto" />
                                </button>
                              );
                            })}
                          </div>

                          {/* Active Pin Info Card Overlay */}
                          {activePin && (
                            <div className="absolute bottom-4 left-4 right-4 md:right-auto md:w-96 bg-white/95 backdrop-blur-md p-4 rounded-2xl border border-sky-200 shadow-2xl space-y-1.5">
                              <div className="flex items-center justify-between">
                                <span className="text-[10px] font-extrabold uppercase tracking-wider px-2.5 py-0.5 rounded-full bg-[#104480] text-white">
                                  {activePin.activityType}
                                </span>
                                <span className="text-[11px] font-mono font-bold text-emerald-700">
                                  {activePin.date} • {activePin.time} WIB
                                </span>
                              </div>
                              <div className="font-extrabold text-sm text-[#0b2545]">{activePin.empName} ({activePin.dept})</div>
                              <div className="text-xs font-bold text-[#104480]">Lokasi: {activePin.clientOrVenue}</div>
                              <p className="text-xs text-slate-600">{activePin.notes}</p>
                              <div className="text-[10px] font-mono text-slate-500 pt-1 border-t">
                                GPS Koordinat: {activePin.lat}, {activePin.lng}
                              </div>
                            </div>
                          )}
                        </div>

                        {/* Tabel Log Lengkap Perjalanan Dinas */}
                        <div className="overflow-x-auto">
                          <table className="w-full text-xs text-left">
                            <thead className="bg-[#0b2545] text-white">
                              <tr>
                                <th className="p-3">Karyawan</th>
                                <th className="p-3">Aktivitas Lapangan</th>
                                <th className="p-3">Lokasi / Klien</th>
                                <th className="p-3">Koordinat GPS</th>
                                <th className="p-3">Waktu Check-in</th>
                                <th className="p-3 text-center">Fokus Peta</th>
                              </tr>
                            </thead>
                            <tbody className="divide-y divide-slate-100">
                              {visiblePins.map(pin => {
                                const meta = FIELD_ACTIVITY_TYPES.find(a => a.id === pin.activityType) || FIELD_ACTIVITY_TYPES[0];
                                return (
                                  <tr key={pin.id} className="hover:bg-sky-50/40">
                                    <td className="p-3 flex items-center gap-2.5">
                                      <img src={pin.photo} alt={pin.empName} className="w-8 h-8 rounded-full object-cover" />
                                      <div>
                                        <div className="font-bold text-[#0b2545]">{pin.empName}</div>
                                        <div className="text-[10px] text-slate-500">{pin.dept}</div>
                                      </div>
                                    </td>
                                    <td className="p-3">
                                      <span className={`px-2.5 py-1 rounded-full text-[10px] font-extrabold ${meta.badge}`}>
                                        {pin.activityType}
                                      </span>
                                    </td>
                                    <td className="p-3">
                                      <div className="font-bold text-[#0b2545]">{pin.clientOrVenue}</div>
                                      <div className="text-[11px] text-slate-500">{pin.notes}</div>
                                    </td>
                                    <td className="p-3 font-mono text-[11px] text-[#104480]">
                                      {pin.lat}, {pin.lng}
                                    </td>
                                    <td className="p-3 font-mono">{pin.date} • {pin.time} WIB</td>
                                    <td className="p-3 text-center">
                                      <button
                                        onClick={() => setSelectedRadarPinId(pin.id)}
                                        className="bg-[#104480] hover:bg-[#0b2545] text-white font-bold px-3 py-1.5 rounded-lg text-[11px]"
                                      >
                                        Lihat Titik
                                      </button>
                                    </td>
                                  </tr>
                                );
                              })}
                            </tbody>
                          </table>
                        </div>
                      </div>
                    );
                  })()}
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB PENGATURAN LOKASI KANTOR & GEOFENCE MAP AKURAT        */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'lokasi-kantor' && (
              <div className="space-y-6">
                <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-5">
                  <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3 border-b pb-4">
                    <div>
                      <h3 className="font-bold text-base text-[#0b2545] flex items-center gap-2">
                        <Building2 className="w-5 h-5 text-[#104480]" /> Pengaturan Alamat Kantor & Titik Koordinat Map Akurat
                      </h3>
                      <p className="text-xs text-slate-500">
                        Edit alamat kantor utama, koordinat Latitude/Longitude, serta radius geofence presensi. Perubahan otomatis tersinkronisasi ke Google Maps Karyawan & Radar HRD.
                      </p>
                    </div>
                    <button
                      type="button"
                      onClick={() => {
                        if (navigator.geolocation) {
                          navigator.geolocation.getCurrentPosition(
                            (pos) => {
                              setOfficeForm({
                                ...officeForm,
                                lat: Number(pos.coords.latitude.toFixed(6)),
                                lng: Number(pos.coords.longitude.toFixed(6))
                              });
                              showToast('Koordinat GPS lokasi Anda saat ini berhasil diambil!');
                            },
                            () => {
                              showToast('Izin lokasi browser tidak aktif. Silakan isi koordinat atau pilih titik cepat.', 'error');
                            },
                            { enableHighAccuracy: true }
                          );
                        }
                      }}
                      className="bg-sky-100 hover:bg-sky-200 text-[#0b2545] text-xs font-bold px-3.5 py-2 rounded-xl flex items-center gap-1.5 border border-sky-200 transition"
                    >
                      <Navigation className="w-3.5 h-3.5 text-[#104480]" />
                      <span>Ambil Titik GPS Saya Saat Ini</span>
                    </button>
                  </div>

                  <div className="grid grid-cols-1 lg:grid-cols-12 gap-6">
                    {/* Form Edit Alamat & Koordinat */}
                    <form
                      onSubmit={(e) => {
                        e.preventDefault();
                        const parsedLat = parseFloat(officeForm.lat);
                        const parsedLng = parseFloat(officeForm.lng);
                        const parsedRad = parseInt(officeForm.radiusMeters, 10) || 250;
                        if (Number.isNaN(parsedLat) || Number.isNaN(parsedLng)) {
                          showToast('Format Latitude dan Longitude harus berupa angka desimal yang valid!', 'error');
                          return;
                        }
                        const updatedLoc = {
                          name: officeForm.name.trim(),
                          address: officeForm.address.trim(),
                          lat: parsedLat,
                          lng: parsedLng,
                          radiusMeters: parsedRad
                        };
                        setOfficeLocation(updatedLoc);
                        setGpsCoords({
                          lat: updatedLoc.lat,
                          lng: updatedLoc.lng,
                          area: updatedLoc.name
                        });
                        showToast('Alamat kantor & koordinat GPS berhasil diperbarui ke seluruh portal!');
                      }}
                      className="lg:col-span-5 space-y-4 text-xs"
                    >
                      <div>
                        <label className="block font-bold text-[#0b2545] mb-1">Nama Kantor / Gedung Utama</label>
                        <input
                          type="text"
                          value={officeForm.name}
                          onChange={(e) => setOfficeForm({ ...officeForm, name: e.target.value })}
                          placeholder="Contoh: Oasis Creative HQ Yogyakarta"
                          className="w-full p-2.5 border border-slate-300 rounded-xl font-semibold focus:ring-2 focus:ring-[#104480]"
                          required
                        />
                      </div>

                      <div>
                        <label className="block font-bold text-[#0b2545] mb-1">Alamat Lengkap Kantor</label>
                        <textarea
                          rows={3}
                          value={officeForm.address}
                          onChange={(e) => setOfficeForm({ ...officeForm, address: e.target.value })}
                          placeholder="Masukkan jalan, kelurahan, kecamatan, kota, dan kode pos..."
                          className="w-full p-2.5 border border-slate-300 rounded-xl focus:ring-2 focus:ring-[#104480]"
                          required
                        />
                      </div>

                      <div className="grid grid-cols-2 gap-3">
                        <div>
                          <label className="block font-bold text-[#0b2545] mb-1">Latitude (Lintang)</label>
                          <input
                            type="number"
                            step="any"
                            value={officeForm.lat}
                            onChange={(e) => setOfficeForm({ ...officeForm, lat: e.target.value })}
                            className="w-full p-2.5 border border-slate-300 rounded-xl font-mono font-bold text-[#104480]"
                            required
                          />
                        </div>
                        <div>
                          <label className="block font-bold text-[#0b2545] mb-1">Longitude (Bujur)</label>
                          <input
                            type="number"
                            step="any"
                            value={officeForm.lng}
                            onChange={(e) => setOfficeForm({ ...officeForm, lng: e.target.value })}
                            className="w-full p-2.5 border border-slate-300 rounded-xl font-mono font-bold text-[#104480]"
                            required
                          />
                        </div>
                      </div>

                      <div>
                        <label className="block font-bold text-[#0b2545] mb-1">Radius Geofence Presensi Kantor (Meter)</label>
                        <input
                          type="number"
                          min="20"
                          max="5000"
                          value={officeForm.radiusMeters}
                          onChange={(e) => setOfficeForm({ ...officeForm, radiusMeters: e.target.value })}
                          className="w-full p-2.5 border border-slate-300 rounded-xl font-mono font-bold"
                          required
                        />
                        <span className="text-[11px] text-slate-500 mt-1 block">
                          Karyawan dalam jarak ≤ {officeForm.radiusMeters} meter otomatis terdeteksi berada di kantor.
                        </span>
                      </div>

                      {/* Pilihan Preset Area Cepat */}
                      <div className="bg-slate-50 p-3 rounded-xl border border-slate-200 space-y-1.5">
                        <div className="text-[11px] font-bold text-slate-600">Pilih Cepat Titik Referensi:</div>
                        <div className="flex flex-wrap gap-1.5">
                          {[
                            { label: 'Umbulharjo HQ', name: 'Oasis Creative HQ (Umbulharjo)', address: 'Jl. Glagahsari No. 45, Warungboto, Umbulharjo, Yogyakarta', lat: -7.8105, lng: 110.3850 },
                            { label: 'Sleman Creative Space', name: 'Oasis Creative Studio Sleman', address: 'Jl. Ring Road Utara, Condongcatur, Depok, Sleman, DIY', lat: -7.7586, lng: 110.3991 },
                            { label: 'Kotabaru Office', name: 'Oasis Executive Office Kotabaru', address: 'Jl. Suroto No. 12, Kotabaru, Gondokusuman, Yogyakarta', lat: -7.7865, lng: 110.3718 }
                          ].map(preset => (
                            <button
                              key={preset.label}
                              type="button"
                              onClick={() =>
                                setOfficeForm({
                                  ...officeForm,
                                  name: preset.name,
                                  address: preset.address,
                                  lat: preset.lat,
                                  lng: preset.lng
                                })
                              }
                              className="px-2.5 py-1 rounded-lg bg-white border border-slate-300 hover:border-[#104480] text-[11px] font-bold text-[#0b2545]"
                            >
                              {preset.label}
                            </button>
                          ))}
                        </div>
                      </div>

                      <button
                        type="submit"
                        className="w-full bg-gradient-to-r from-[#0b2545] to-[#104480] hover:opacity-95 text-white font-bold py-3 rounded-xl shadow-md flex items-center justify-center gap-2 transition"
                      >
                        <CheckCircle className="w-4 h-4 text-sky-300" />
                        <span>Simpan & Terapkan Alamat Kantor</span>
                      </button>
                    </form>

                    {/* Live Preview Google Maps Akurat */}
                    <div className="lg:col-span-7 flex flex-col justify-between space-y-3">
                      <div className="flex justify-between items-center">
                        <span className="text-xs font-extrabold text-[#0b2545]">
                          Pratinjau Langsung Google Maps (Zoom Presisi 18x)
                        </span>
                        <a
                          href={`https://www.google.com/maps/search/?api=1&query=${officeForm.lat},${officeForm.lng}`}
                          target="_blank"
                          rel="noreferrer"
                          className="text-xs font-bold text-[#104480] hover:underline flex items-center gap-1"
                        >
                          <span>Buka di Google Maps Penuh ↗</span>
                        </a>
                      </div>

                      <div className="rounded-2xl h-[380px] border-2 border-[#104480]/30 overflow-hidden shadow-inner relative bg-slate-100">
                        <iframe
                          title="Pratinjau Alamat Kantor HRD"
                          width="100%"
                          height="100%"
                          style={{ border: 0 }}
                          loading="lazy"
                          referrerPolicy="no-referrer-when-downgrade"
                          src={`https://maps.google.com/maps?q=${officeForm.lat || -7.8105},${officeForm.lng || 110.3850}&z=18&output=embed`}
                        />

                        <div className="absolute bottom-3 left-3 right-3 bg-white/95 backdrop-blur-md p-3.5 rounded-xl border border-sky-200 shadow-lg flex flex-col sm:flex-row justify-between items-start sm:items-center gap-2">
                          <div>
                            <div className="font-extrabold text-xs text-[#0b2545]">{officeForm.name}</div>
                            <div className="text-[11px] text-slate-600">{officeForm.address}</div>
                            <div className="font-mono text-[10px] text-[#104480] mt-0.5">
                              Titik Pin: {officeForm.lat}, {officeForm.lng} • Radius Geofence: {officeForm.radiusMeters}m
                            </div>
                          </div>
                          <span className="px-2.5 py-1 rounded-full text-[10px] font-bold bg-emerald-100 text-emerald-800 whitespace-nowrap">
                            Pin Akurat Terkunci
                          </span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 2: REKAP PRESENSI MASTER & DOWNLOAD SPREADSHEET        */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'rekap-absent' && (
              <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-5">
                <div className="flex flex-col lg:flex-row justify-between items-start lg:items-center gap-4 border-b pb-4">
                  <div>
                    <h3 className="font-bold text-base text-[#0b2545]">Master Rekap Presensi, Override Jam & Export Spreadsheet</h3>
                    <p className="text-xs text-slate-500">Filter berdasarkan bulan atau divisi, lalu unduh laporan presensi langsung dalam format Excel (.xls) atau CSV.</p>
                  </div>

                  {/* Tombol Download Spreadsheet Otomatis (Excel & CSV) */}
                  <div className="flex flex-wrap items-center gap-2">
                    <button
                      onClick={() => handleDownloadAttendanceSpreadsheet('xls')}
                      className="bg-emerald-600 hover:bg-emerald-700 text-white text-xs font-bold px-4 py-2.5 rounded-xl shadow flex items-center gap-1.5 transition"
                    >
                      <FileSpreadsheet className="w-4 h-4" />
                      <span>Download Excel (.xls)</span>
                    </button>
                    <button
                      onClick={() => handleDownloadAttendanceSpreadsheet('csv')}
                      className="bg-[#104480] hover:bg-[#0b2545] text-white text-xs font-bold px-4 py-2.5 rounded-xl shadow flex items-center gap-1.5 transition"
                    >
                      <Download className="w-4 h-4" />
                      <span>Download CSV (.csv)</span>
                    </button>
                  </div>
                </div>

                {/* Filter Bar Presensi */}
                <div className="grid grid-cols-1 sm:grid-cols-3 gap-3 bg-sky-50/70 p-3.5 rounded-xl border border-sky-100 text-xs">
                  <div>
                    <label className="block font-bold text-[#0b2545] mb-1">Filter Bulan Presensi</label>
                    <input
                      type="month"
                      value={attendanceFilterMonth === 'ALL' ? '' : attendanceFilterMonth}
                      onChange={(e) => setAttendanceFilterMonth(e.target.value || 'ALL')}
                      className="w-full p-2 border rounded-lg bg-white"
                    />
                  </div>
                  <div>
                    <label className="block font-bold text-[#0b2545] mb-1">Filter Divisi / Departemen</label>
                    <select
                      value={attendanceFilterDept}
                      onChange={(e) => setAttendanceFilterDept(e.target.value)}
                      className="w-full p-2 border rounded-lg bg-white font-semibold"
                    >
                      <option value="ALL">Semua Divisi ({records.filter(r => r.category === 'Absensi').length} Log)</option>
                      {DIVISIONS.map(d => <option key={d} value={d}>{d}</option>)}
                    </select>
                  </div>
                  <div className="flex items-end">
                    <button
                      type="button"
                      onClick={() => {
                        setAttendanceFilterMonth('ALL');
                        setAttendanceFilterDept('ALL');
                      }}
                      className="w-full py-2 bg-white border border-slate-300 rounded-lg font-bold text-slate-600 hover:bg-slate-100"
                    >
                      Reset Filter Presensi
                    </button>
                  </div>
                </div>

                <div className="overflow-x-auto">
                  <table className="w-full text-xs text-left">
                    <thead className="bg-[#0b2545] text-white">
                      <tr>
                        <th className="p-3">Karyawan</th>
                        <th className="p-3">Divisi</th>
                        <th className="p-3">Tanggal</th>
                        <th className="p-3">Masuk - Pulang</th>
                        <th className="p-3">Lokasi GPS</th>
                        <th className="p-3">Status / Denda</th>
                        <th className="p-3 text-center">Edit HRD</th>
                      </tr>
                    </thead>
                    <tbody className="divide-y divide-slate-100">
                      {filteredAttendanceLogs.length === 0 ? (
                        <tr>
                          <td colSpan="7" className="p-6 text-center text-slate-400">Tidak ada data presensi pada periode/divisi ini.</td>
                        </tr>
                      ) : (
                        filteredAttendanceLogs.map(rec => (
                          <tr key={rec.id} className="hover:bg-slate-50">
                            <td className="p-3 font-bold text-[#0b2545]">
                              {rec.empName}
                              <span className="block text-[10px] font-mono text-slate-400">{rec.empId}</span>
                            </td>
                            <td className="p-3 text-slate-600">{rec.dept}</td>
                            <td className="p-3 font-mono">{rec.date}</td>
                            <td className="p-3 font-mono font-bold">{rec.clockIn} - {rec.clockOut}</td>
                            <td className="p-3 text-slate-600">{rec.location}</td>
                            <td className="p-3">
                              {rec.overrideByAdmin ? (
                                <span className="bg-emerald-100 text-emerald-800 font-bold px-2.5 py-0.5 rounded-full text-[10px]">
                                  Dispensasi HRD
                                </span>
                              ) : rec.lateMinutes > 0 ? (
                                <span className="text-rose-600 font-bold">
                                  Terlambat {rec.lateMinutes}m (Rp {(rec.lateMinutes * 800).toLocaleString('id-ID')})
                                </span>
                              ) : (
                                <span className="text-emerald-600 font-bold">Tepat Waktu</span>
                              )}
                            </td>
                            <td className="p-3 text-center">
                              <button
                                onClick={() => {
                                  setOverrideTarget(rec);
                                  setOverrideClockIn(rec.clockIn);
                                  setOverrideClockOut(rec.clockOut);
                                }}
                                className="bg-[#104480] text-white font-bold px-3 py-1 rounded-lg text-[11px]"
                              >
                                Edit / Override
                              </button>
                            </td>
                          </tr>
                        ))
                      )}
                    </tbody>
                  </table>
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 3: KALENDER AGENDA & RAPAT HRD INTERAKTIF             */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'kalender-hrd' && (
              <div className="space-y-6">
                <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-4">
                  <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3">
                    <div>
                      <h3 className="font-bold text-base text-[#0b2545] flex items-center gap-2">
                        <Calendar className="w-5 h-5 text-[#104480]" /> Kalender Rapat & Koordinasi HRD
                      </h3>
                      <p className="text-xs text-slate-500">Jadwalkan, filter, dan kelola rapat koordinasi, interview, pleno, dan audit HRD.</p>
                    </div>
                    <button
                      onClick={() => {
                        setEditingAgenda(null);
                        setAgendaForm({
                          date: '2026-11-12',
                          startTime: '09:00',
                          endTime: '10:30',
                          title: '',
                          category: 'Koordinasi Internal',
                          description: '',
                          location: 'Ruang Meeting HRD 1'
                        });
                        setShowAgendaModal(true);
                      }}
                      className="bg-[#104480] hover:bg-[#1D6CB0] text-white text-xs font-bold px-4 py-2.5 rounded-xl shadow flex items-center gap-1.5"
                    >
                      <Plus className="w-4 h-4" />
                      <span>Tambah Rapat / Agenda</span>
                    </button>
                  </div>

                  <div className="grid grid-cols-1 sm:grid-cols-4 gap-3 bg-sky-50/70 p-3.5 rounded-xl border border-sky-100 text-xs">
                    <div>
                      <label className="block font-bold text-[#0b2545] mb-1">Filter Tanggal</label>
                      <input
                        type="date"
                        value={filterAgendaDate}
                        onChange={(e) => setFilterAgendaDate(e.target.value)}
                        className="w-full p-2 border rounded-lg bg-white"
                      />
                    </div>
                    <div>
                      <label className="block font-bold text-[#0b2545] mb-1">Filter Jam Mulai</label>
                      <input
                        type="text"
                        placeholder="Contoh: 09:00"
                        value={filterAgendaTime}
                        onChange={(e) => setFilterAgendaTime(e.target.value)}
                        className="w-full p-2 border rounded-lg bg-white"
                      />
                    </div>
                    <div>
                      <label className="block font-bold text-[#0b2545] mb-1">Cari Nama Agenda</label>
                      <input
                        type="text"
                        placeholder="Rapat, Koordinasi, Audit..."
                        value={filterAgendaQuery}
                        onChange={(e) => setFilterAgendaQuery(e.target.value)}
                        className="w-full p-2 border rounded-lg bg-white"
                      />
                    </div>
                    <div className="flex items-end">
                      <button
                        type="button"
                        onClick={() => {
                          setFilterAgendaDate('');
                          setFilterAgendaTime('');
                          setFilterAgendaQuery('');
                        }}
                        className="w-full py-2 bg-white border border-slate-300 rounded-lg font-bold text-slate-600 hover:bg-slate-100"
                      >
                        Reset Filter
                      </button>
                    </div>
                  </div>
                </div>

                <div className="grid grid-cols-1 lg:grid-cols-3 gap-6">
                  <div className="lg:col-span-2 bg-white rounded-2xl p-5 shadow-sm border border-slate-200 space-y-4">
                    <div className="flex justify-between items-center">
                      <h4 className="font-extrabold text-sm text-[#0b2545]">
                        {calMonth.toLocaleDateString('id-ID', { month: 'long', year: 'numeric' })}
                      </h4>
                      <div className="flex gap-1.5">
                        <button
                          onClick={() => setCalMonth(new Date(calMonth.getFullYear(), calMonth.getMonth() - 1, 1))}
                          className="p-1.5 border rounded-lg hover:bg-slate-100"
                        >
                          <ChevronLeft className="w-4 h-4" />
                        </button>
                        <button
                          onClick={() => setCalMonth(new Date(calMonth.getFullYear(), calMonth.getMonth() + 1, 1))}
                          className="p-1.5 border rounded-lg hover:bg-slate-100"
                        >
                          <ChevronRight className="w-4 h-4" />
                        </button>
                      </div>
                    </div>

                    <div className="grid grid-cols-7 gap-1 text-center text-[11px] font-bold text-slate-500 pb-1 border-b">
                      {['Min', 'Sen', 'Sel', 'Rab', 'Kam', 'Jum', 'Sab'].map(d => <div key={d}>{d}</div>)}
                    </div>

                    <div className="grid grid-cols-7 gap-1.5">
                      {calendarDays.map((cell, idx) => {
                        if (!cell) return <div key={idx} className="h-20 bg-slate-50/50 rounded-xl" />;
                        const dayAgendas = hrdAgendas.filter(a => a.date === cell.dateStr);
                        const isSelected = filterAgendaDate === cell.dateStr;
                        return (
                          <div
                            key={cell.dateStr}
                            onClick={() => setFilterAgendaDate(isSelected ? '' : cell.dateStr)}
                            className={`h-20 p-1.5 rounded-xl border text-left cursor-pointer transition overflow-hidden flex flex-col justify-between ${
                              isSelected ? 'border-[#104480] bg-sky-50 ring-2 ring-[#104480]/20' : 'border-slate-200 hover:border-sky-300 bg-white'
                            }`}
                          >
                            <span className="text-xs font-bold text-slate-700">{cell.day}</span>
                            <div className="space-y-0.5 overflow-y-auto">
                              {dayAgendas.map(a => (
                                <div key={a.id} className="text-[9px] font-bold bg-[#104480] text-white px-1.5 py-0.5 rounded truncate">
                                  {a.startTime} {a.title}
                                </div>
                              ))}
                            </div>
                          </div>
                        );
                      })}
                    </div>
                  </div>

                  <div className="bg-white rounded-2xl p-5 shadow-sm border border-slate-200 space-y-3">
                    <h4 className="font-bold text-sm text-[#0b2545] border-b pb-2">
                      Daftar Jadwal Rapat & Koordinasi ({filteredAgendas.length})
                    </h4>
                    <div className="space-y-3 max-h-[420px] overflow-y-auto pr-1">
                      {filteredAgendas.length === 0 ? (
                        <p className="text-xs text-slate-400 text-center py-6">Tidak ada agenda yang sesuai filter.</p>
                      ) : (
                        filteredAgendas.map(ag => (
                          <div key={ag.id} className="p-3.5 rounded-xl border border-sky-100 bg-sky-50/40 space-y-1.5">
                            <div className="flex justify-between items-center">
                              <span className="text-[10px] font-bold bg-[#104480] text-white px-2 py-0.5 rounded-full">
                                {ag.category}
                              </span>
                              <span className="text-[11px] font-mono font-bold text-[#104480]">
                                {ag.date} | {ag.startTime}-{ag.endTime}
                              </span>
                            </div>
                            <h5 className="font-bold text-xs text-[#0b2545]">{ag.title}</h5>
                            <p className="text-[11px] text-slate-600">{ag.description}</p>
                            <div className="text-[10px] text-slate-500 font-semibold">Lokasi: {ag.location}</div>
                            <div className="flex justify-end gap-2 pt-1.5 border-t border-sky-100">
                              <button
                                onClick={() => {
                                  setEditingAgenda(ag);
                                  setAgendaForm(ag);
                                  setShowAgendaModal(true);
                                }}
                                className="text-[#104480] hover:underline font-bold text-[11px] flex items-center gap-0.5"
                              >
                                <Edit className="w-3 h-3" /> Edit
                              </button>
                              <button
                                onClick={() => {
                                  setHrdAgendas(hrdAgendas.filter(item => item.id !== ag.id));
                                  showToast('Agenda rapat dihapus.');
                                }}
                                className="text-rose-600 hover:underline font-bold text-[11px] flex items-center gap-0.5"
                              >
                                <Trash2 className="w-3 h-3" /> Hapus
                              </button>
                            </div>
                          </div>
                        ))
                      )}
                    </div>
                  </div>
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 4: MASTER DATA KARYAWAN (FULL EDIT + FOTO + PASSWORD) */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'master-emp' && (
              <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-5">
                <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3">
                  <div>
                    <h3 className="font-bold text-base text-[#0b2545]">Kelola Master Data Karyawan (Full Editable)</h3>
                    <p className="text-xs text-slate-500">Edit foto, ID, nama lengkap, nomor HP, rekening, jabatan, gaji, & password akses.</p>
                  </div>
                  <div className="flex items-center gap-2 w-full sm:w-auto">
                    <div className="relative flex-1 sm:w-56">
                      <Search className="w-3.5 h-3.5 text-slate-400 absolute left-3 top-2.5" />
                      <input
                        type="text"
                        placeholder="Cari nama / ID..."
                        value={empSearch}
                        onChange={(e) => setEmpSearch(e.target.value)}
                        className="w-full pl-8 pr-3 py-2 text-xs border rounded-xl"
                      />
                    </div>
                    <button
                      onClick={() => {
                        setEditingEmpId(null);
                        setEmpForm({
                          id: `EMP00${employees.length + 1}`,
                          name: '',
                          dept: DIVISIONS[0],
                          role: '',
                          phone: '+62 812-',
                          bank: 'BCA - ',
                          baseSalary: 7000000,
                          allowances: 1000000,
                          password: '',
                          photo: 'https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?w=150&auto=format&fit=crop&q=80',
                          kpiScore: 85
                        });
                        setShowEmpModal(true);
                      }}
                      className="bg-[#104480] hover:bg-[#1D6CB0] text-white text-xs font-bold px-4 py-2 rounded-xl flex items-center gap-1.5 whitespace-nowrap"
                    >
                      <UserPlus className="w-4 h-4" /> Tambah Karyawan
                    </button>
                  </div>
                </div>

                <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                  {filteredEmployees.map(emp => (
                    <div key={emp.id} className="border border-slate-200 rounded-2xl p-4 bg-slate-50/50 hover:border-[#104480] transition space-y-3">
                      <div className="flex items-center gap-3">
                        <img
                          src={emp.photo || 'https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?w=150&auto=format&fit=crop&q=80'}
                          alt={emp.name}
                          className="w-14 h-14 rounded-2xl object-cover border-2 border-[#104480]/30 shadow-sm"
                        />
                        <div>
                          <span className="font-mono text-[10px] font-bold bg-[#104480] text-white px-2 py-0.5 rounded">
                            {emp.id}
                          </span>
                          <h4 className="font-bold text-sm text-[#0b2545] mt-1">{emp.name}</h4>
                          <p className="text-xs text-[#104480] font-semibold">{emp.role}</p>
                        </div>
                      </div>

                      <div className="bg-white p-3 rounded-xl border border-slate-100 text-xs space-y-1 text-slate-600">
                        <p><strong>Divisi:</strong> {emp.dept}</p>
                        <p className="flex items-center gap-1"><Phone className="w-3 h-3 text-[#104480]" /> {emp.phone}</p>
                        <p className="flex items-center gap-1"><CreditCard className="w-3 h-3 text-[#104480]" /> {emp.bank}</p>
                        <p><strong>Gaji Pokok:</strong> Rp {Number(emp.baseSalary).toLocaleString('id-ID')}</p>
                        <p><strong>Password Portal:</strong> <span className="font-mono font-bold text-[#0b2545]">{emp.password}</span></p>
                      </div>

                      <div className="flex justify-end gap-2 pt-1">
                        <button
                          onClick={() => {
                            setEditingEmpId(emp.id);
                            setEmpForm(emp);
                            setShowEmpModal(true);
                          }}
                          className="bg-[#104480] hover:bg-[#1D6CB0] text-white text-xs font-bold px-3 py-1.5 rounded-lg flex items-center gap-1"
                        >
                          <Edit className="w-3.5 h-3.5" /> Edit Semua Data
                        </button>
                        <button
                          onClick={() => setConfirmDeleteEmp(emp)}
                          className="bg-rose-600 hover:bg-rose-700 text-white text-xs font-bold px-3 py-1.5 rounded-lg"
                        >
                          <Trash2 className="w-3.5 h-3.5" />
                        </button>
                      </div>
                    </div>
                  ))}
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 5: OASIS KPI SYSTEM & HALL OF FAME (EDITABLE)         */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'kpi' && (
              <div className="space-y-6">
                <div className="bg-gradient-to-r from-[#07182e] via-[#0b2545] to-[#104480] rounded-3xl p-6 text-white shadow-xl space-y-4">
                  <div className="flex justify-between items-center border-b border-white/15 pb-3">
                    <h3 className="font-extrabold text-base flex items-center gap-2">
                      <Sparkles className="w-5 h-5 text-sky-300" /> Hall of Fame - Karyawan Terbaik Bulanan
                    </h3>
                    <span className="text-xs font-bold bg-white/15 px-3 py-1 rounded-full">Auto-Ranking KPI</span>
                  </div>
                  <div className="grid grid-cols-1 md:grid-cols-3 gap-4">
                    {topPerformers.map((emp, idx) => (
                      <div key={emp.id} className="bg-white/10 backdrop-blur-sm rounded-2xl p-4 border border-white/20 flex items-center gap-3 relative">
                        <div className="w-8 h-8 rounded-full bg-sky-400 text-[#07182e] font-black flex items-center justify-center text-xs shadow">
                          #{idx + 1}
                        </div>
                        <img src={emp.photo} alt={emp.name} className="w-12 h-12 rounded-full object-cover border-2 border-sky-300" />
                        <div>
                          <h4 className="font-bold text-sm">{emp.name}</h4>
                          <p className="text-[11px] text-sky-200">{emp.dept}</p>
                          <span className="inline-block mt-1 bg-sky-400 text-[#07182e] font-extrabold text-[10px] px-2.5 py-0.5 rounded-full">
                            Skor KPI: {emp.kpiScore} / 100
                          </span>
                        </div>
                      </div>
                    ))}
                  </div>
                </div>

                <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-4">
                  <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3">
                    <div>
                      <h3 className="font-bold text-base text-[#0b2545]">Rekap & Edit Nilai KPI Karyawan</h3>
                      <p className="text-xs text-slate-500">Klik tombol Edit Nilai untuk memperbarui skor kinerja karyawan secara langsung.</p>
                    </div>
                    <select
                      value={kpiDeptFilter}
                      onChange={(e) => setKpiDeptFilter(e.target.value)}
                      className="border rounded-xl px-3 py-2 text-xs font-bold text-[#0b2545]"
                    >
                      <option value="ALL">Semua Divisi</option>
                      {DIVISIONS.map(d => <option key={d} value={d}>{d}</option>)}
                    </select>
                  </div>

                  <div className="overflow-x-auto">
                    <table className="w-full text-xs text-left">
                      <thead className="bg-[#0b2545] text-white">
                        <tr>
                          <th className="p-3">Karyawan</th>
                          <th className="p-3">Divisi</th>
                          <th className="p-3">Predikat</th>
                          <th className="p-3">Nilai KPI (0-100)</th>
                          <th className="p-3 text-center">Edit Nilai</th>
                        </tr>
                      </thead>
                      <tbody className="divide-y divide-slate-100">
                        {filteredKpiEmployees.map(emp => (
                          <tr key={emp.id} className="hover:bg-slate-50">
                            <td className="p-3 flex items-center gap-2.5">
                              <img src={emp.photo} alt={emp.name} className="w-8 h-8 rounded-full object-cover" />
                              <div>
                                <div className="font-bold text-[#0b2545]">{emp.name}</div>
                                <div className="text-[10px] font-mono text-slate-400">{emp.id}</div>
                              </div>
                            </td>
                            <td className="p-3">{emp.dept}</td>
                            <td className="p-3">
                              <span className={`px-2.5 py-0.5 rounded-full text-[10px] font-bold ${
                                emp.kpiScore >= 95 ? 'bg-sky-100 text-[#104480]' : 'bg-emerald-100 text-emerald-800'
                              }`}>
                                {emp.kpiScore >= 95 ? 'Outstanding Performer' : 'Good Performer'}
                              </span>
                            </td>
                            <td className="p-3 font-mono font-extrabold text-sm text-[#104480]">
                              {editingKpiId === emp.id ? (
                                <input
                                  type="number"
                                  min="0"
                                  max="100"
                                  value={tempKpiVal}
                                  onChange={(e) => setTempKpiVal(Number(e.target.value))}
                                  className="w-20 border-2 border-[#104480] rounded-lg px-2 py-1 font-bold"
                                />
                              ) : (
                                emp.kpiScore
                              )}
                            </td>
                            <td className="p-3 text-center">
                              {editingKpiId === emp.id ? (
                                <button
                                  onClick={() => {
                                    setEmployees(employees.map(item => item.id === emp.id ? { ...item, kpiScore: tempKpiVal } : item));
                                    setEditingKpiId(null);
                                    showToast(`Nilai KPI ${emp.name} diperbarui.`);
                                  }}
                                  className="bg-emerald-600 text-white font-bold px-3 py-1 rounded-lg text-[11px]"
                                >
                                  Simpan
                                </button>
                              ) : (
                                <button
                                  onClick={() => {
                                    setEditingKpiId(emp.id);
                                    setTempKpiVal(emp.kpiScore);
                                  }}
                                  className="bg-[#104480] text-white font-bold px-3 py-1 rounded-lg text-[11px]"
                                >
                                  Edit Nilai
                                </button>
                              )}
                            </td>
                          </tr>
                        ))}
                      </tbody>
                    </table>
                  </div>
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 6: REKRUTMEN, INTERVIEW & SKILL TEST KANDIDAT         */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'rekrutmen' && (
              <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-5">
                <div className="flex justify-between items-center">
                  <div>
                    <h3 className="font-bold text-base text-[#0b2545]">Rekrutmen, Jadwal Interview & Penilaian Skill Test</h3>
                    <p className="text-xs text-slate-500">Catat kandidat, input skor interview & skill test, serta tentukan keputusan lolos atau rejection.</p>
                  </div>
                  <button
                    onClick={() => setShowCandModal(true)}
                    className="bg-[#104480] hover:bg-[#1D6CB0] text-white text-xs font-bold px-4 py-2 rounded-xl flex items-center gap-1.5"
                  >
                    <Plus className="w-4 h-4" /> Tambah Kandidat
                  </button>
                </div>

                <div className="overflow-x-auto">
                  <table className="w-full text-xs text-left">
                    <thead className="bg-[#0b2545] text-white">
                      <tr>
                        <th className="p-3">Nama Kandidat & Posisi</th>
                        <th className="p-3">Tgl Interview</th>
                        <th className="p-3">Skor Interview</th>
                        <th className="p-3">Skor Skill Test</th>
                        <th className="p-3">Catatan HRD</th>
                        <th className="p-3">Status Tahapan</th>
                        <th className="p-3 text-center">Keputusan</th>
                      </tr>
                    </thead>
                    <tbody className="divide-y divide-slate-100">
                      {candidates.map(c => (
                        <tr key={c.id} className="hover:bg-slate-50">
                          <td className="p-3">
                            <div className="font-bold text-[#0b2545]">{c.name}</div>
                            <div className="text-[11px] text-[#104480] font-semibold">{c.position}</div>
                          </td>
                          <td className="p-3 font-mono">{c.interviewDate}</td>
                          <td className="p-3 font-mono font-bold">{c.interviewScore}</td>
                          <td className="p-3 font-mono font-bold">{c.skillTestScore}</td>
                          <td className="p-3 max-w-xs">{c.notes}</td>
                          <td className="p-3">
                            <span className={`px-2.5 py-1 rounded-full text-[10px] font-bold ${
                              c.stage === 'Lolos Tahap Selanjutnya' ? 'bg-emerald-100 text-emerald-800' :
                              c.stage === 'Rejected' ? 'bg-rose-100 text-rose-800' : 'bg-amber-100 text-amber-800'
                            }`}>
                              {c.stage}
                            </span>
                          </td>
                          <td className="p-3 text-center">
                            <div className="flex justify-center gap-1.5">
                              <button
                                onClick={() => setCandidates(candidates.map(item => item.id === c.id ? { ...item, stage: 'Lolos Tahap Selanjutnya' } : item))}
                                className="bg-emerald-600 text-white font-bold px-2.5 py-1 rounded-lg text-[10px]"
                              >
                                Lolos Next Stage
                              </button>
                              <button
                                onClick={() => setCandidates(candidates.map(item => item.id === c.id ? { ...item, stage: 'Rejected' } : item))}
                                className="bg-rose-600 text-white font-bold px-2.5 py-1 rounded-lg text-[10px]"
                              >
                                Reject
                              </button>
                            </div>
                          </td>
                        </tr>
                      ))}
                    </tbody>
                  </table>
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 7: TO-DO LIST HRD (FILTER PRIORITAS & WEEKLY/MONTHLY) */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'tasks' && (
              <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-5">
                <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3">
                  <div>
                    <h3 className="font-bold text-base text-[#0b2545]">To-Do List Operasional HRD</h3>
                    <p className="text-xs text-slate-500">Filter berdasarkan prioritas (Urgent, Sedang, Low) dan rekapan Weekly / Monthly.</p>
                  </div>

                  <div className="flex flex-wrap gap-2 text-xs">
                    <select
                      value={taskPriorityFilter}
                      onChange={(e) => setTaskPriorityFilter(e.target.value)}
                      className="border rounded-xl px-3 py-1.5 font-bold text-[#0b2545]"
                    >
                      <option value="ALL">Semua Prioritas</option>
                      <option value="Urgent">Prioritas Urgent</option>
                      <option value="Sedang">Prioritas Sedang</option>
                      <option value="Low">Prioritas Low</option>
                    </select>
                    <select
                      value={taskPeriodFilter}
                      onChange={(e) => setTaskPeriodFilter(e.target.value)}
                      className="border rounded-xl px-3 py-1.5 font-bold text-[#0b2545]"
                    >
                      <option value="ALL">Semua Periode</option>
                      <option value="Weekly">Rekap Weekly</option>
                      <option value="Monthly">Rekap Monthly</option>
                    </select>
                  </div>
                </div>

                <form
                  onSubmit={(e) => {
                    e.preventDefault();
                    if (!newTaskForm.title) return;
                    setHrdTasks([
                      { id: `TSK-${Date.now()}`, ...newTaskForm, status: 'To-Do' },
                      ...hrdTasks
                    ]);
                    setNewTaskForm({ ...newTaskForm, title: '' });
                    showToast('Tugas HRD ditambahkan.');
                  }}
                  className="grid grid-cols-1 sm:grid-cols-5 gap-2 bg-sky-50 p-3 rounded-xl border border-sky-100 text-xs"
                >
                  <input
                    type="text"
                    placeholder="Judul tugas HRD baru..."
                    value={newTaskForm.title}
                    onChange={(e) => setNewTaskForm({ ...newTaskForm, title: e.target.value })}
                    className="sm:col-span-2 p-2 border rounded-lg bg-white"
                    required
                  />
                  <select
                    value={newTaskForm.priority}
                    onChange={(e) => setNewTaskForm({ ...newTaskForm, priority: e.target.value })}
                    className="p-2 border rounded-lg bg-white font-semibold"
                  >
                    <option value="Urgent">Urgent</option>
                    <option value="Sedang">Sedang</option>
                    <option value="Low">Low</option>
                  </select>
                  <select
                    value={newTaskForm.period}
                    onChange={(e) => setNewTaskForm({ ...newTaskForm, period: e.target.value })}
                    className="p-2 border rounded-lg bg-white font-semibold"
                  >
                    <option value="Weekly">Weekly</option>
                    <option value="Monthly">Monthly</option>
                  </select>
                  <button type="submit" className="bg-[#104480] text-white font-bold rounded-lg px-3 py-2">
                    + Tambah Task
                  </button>
                </form>

                <div className="grid grid-cols-1 md:grid-cols-3 gap-4">
                  {filteredTasks.map(task => (
                    <div key={task.id} className="p-4 rounded-2xl border border-slate-200 bg-slate-50/70 space-y-2">
                      <div className="flex justify-between items-center">
                        <span className={`text-[10px] font-bold px-2.5 py-0.5 rounded-full ${
                          task.priority === 'Urgent' ? 'bg-rose-100 text-rose-700' :
                          task.priority === 'Sedang' ? 'bg-amber-100 text-amber-800' : 'bg-sky-100 text-[#104480]'
                        }`}>
                          {task.priority}
                        </span>
                        <span className="text-[10px] font-bold text-slate-500">{task.period}</span>
                      </div>
                      <h4 className="font-bold text-xs text-[#0b2545]">{task.title}</h4>
                      <div className="flex justify-between items-center pt-2 border-t text-[11px]">
                        <span className="font-semibold text-[#104480]">{task.status}</span>
                        <div className="flex gap-2">
                          {task.status !== 'Done' && (
                            <button
                              onClick={() => setHrdTasks(hrdTasks.map(t => t.id === task.id ? { ...t, status: 'Done' } : t))}
                              className="text-emerald-600 font-bold hover:underline"
                            >
                              Selesai
                            </button>
                          )}
                          <button
                            onClick={() => setHrdTasks(hrdTasks.filter(t => t.id !== task.id))}
                            className="text-rose-600 font-bold hover:underline"
                          >
                            Hapus
                          </button>
                        </div>
                      </div>
                    </div>
                  ))}
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 8: PENGUMUMAN INTERNAL TERINTEGRASI KE AKUN KARYAWAN  */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'pengumuman' && (
              <div className="grid grid-cols-1 lg:grid-cols-3 gap-6">
                <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-4">
                  <h3 className="font-bold text-base text-[#0b2545]">Buat Pengumuman Baru</h3>
                  <p className="text-xs text-slate-500">Pengumuman yang diterbitkan otomatis tampil live di Portal seluruh Karyawan.</p>
                  <form
                    onSubmit={(e) => {
                      e.preventDefault();
                      const created = {
                        id: `ANN-${Date.now()}`,
                        date: nowTime.toISOString().split('T')[0],
                        ...annForm
                      };
                      setAnnouncements([created, ...announcements]);
                      setAnnForm({ title: '', priority: 'Penting', content: '' });
                      showToast('Pengumuman diterbitkan dan tampil live di portal karyawan!');
                    }}
                    className="space-y-3 text-xs"
                  >
                    <div>
                      <label className="block font-bold mb-1">Judul Pengumuman</label>
                      <input
                        type="text"
                        value={annForm.title}
                        onChange={(e) => setAnnForm({ ...annForm, title: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                        required
                      />
                    </div>
                    <div>
                      <label className="block font-bold mb-1">Kategori / Prioritas</label>
                      <select
                        value={annForm.priority}
                        onChange={(e) => setAnnForm({ ...annForm, priority: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                      >
                        <option value="Penting">Penting / Urgent</option>
                        <option value="Info Umum">Info Umum</option>
                      </select>
                    </div>
                    <div>
                      <label className="block font-bold mb-1">Isi Pengumuman</label>
                      <textarea
                        rows={3}
                        value={annForm.content}
                        onChange={(e) => setAnnForm({ ...annForm, content: e.target.value })}
                        className="w-full p-2.5 border rounded-xl"
                        required
                      />
                    </div>
                    <button type="submit" className="w-full bg-[#104480] hover:bg-[#1D6CB0] text-white font-bold py-2.5 rounded-xl">
                      Terbitkan ke Portal Karyawan
                    </button>
                  </form>
                </div>

                <div className="lg:col-span-2 bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-4">
                  <h3 className="font-bold text-base text-[#0b2545]">Daftar Pengumuman Tayang ({announcements.length})</h3>
                  <div className="space-y-3">
                    {announcements.map(ann => (
                      <div key={ann.id} className="p-4 rounded-2xl border border-sky-100 bg-sky-50/50 flex justify-between items-start gap-3">
                        <div className="space-y-1">
                          <div className="flex items-center gap-2">
                            <span className="text-[10px] font-bold bg-[#104480] text-white px-2.5 py-0.5 rounded-full">
                              {ann.priority}
                            </span>
                            <span className="text-[11px] font-mono text-slate-500">{ann.date}</span>
                          </div>
                          <h4 className="font-bold text-sm text-[#0b2545]">{ann.title}</h4>
                          <p className="text-xs text-slate-600">{ann.content}</p>
                        </div>
                        <button
                          onClick={() => setAnnouncements(announcements.filter(a => a.id !== ann.id))}
                          className="text-rose-600 hover:bg-rose-50 p-1.5 rounded-lg"
                        >
                          <Trash2 className="w-4 h-4" />
                        </button>
                      </div>
                    ))}
                  </div>
                </div>
              </div>
            )}

            {/* ------------------------------------------------------------- */}
            {/* HRD TAB 9: REKAP GAJI, DENDA & SLIP GAJI                      */}
            {/* ------------------------------------------------------------- */}
            {hrdTab === 'payroll' && (
              <div className="bg-white rounded-2xl p-6 shadow-sm border border-slate-200 space-y-6">
                <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3 border-b pb-4">
                  <div>
                    <h3 className="font-bold text-base text-[#0b2545]">Rekapitulasi Gaji & Pemotongan Absensi</h3>
                    <p className="text-xs text-slate-500">Perhitungan otomatis berdasarkan Gaji Pokok, Tunjangan, Bonus KPI, dan Denda Absensi.</p>
                  </div>
                  <select
                    value={payrollEmpId}
                    onChange={(e) => setPayrollEmpId(e.target.value)}
                    className="border-2 border-[#104480] rounded-xl px-3 py-2 text-xs font-bold text-[#0b2545]"
                  >
                    {employees.map(e => <option key={e.id} value={e.id}>{e.name} ({e.id})</option>)}
                  </select>
                </div>

                <div className="grid grid-cols-1 md:grid-cols-2 gap-6 text-xs">
                  <div className="p-4 rounded-2xl bg-sky-50/70 border border-sky-200 space-y-2">
                    <h4 className="font-bold text-[#0b2545] border-b border-sky-200 pb-2">Penerimaan (Gross Income)</h4>
                    <div className="flex justify-between"><span>Gaji Pokok:</span><span className="font-mono">Rp {Number(selectedPayrollData.emp.baseSalary).toLocaleString('id-ID')}</span></div>
                    <div className="flex justify-between"><span>Tunjangan:</span><span className="font-mono">Rp {Number(selectedPayrollData.emp.allowances).toLocaleString('id-ID')}</span></div>
                    <div className="flex justify-between"><span>Bonus Performance KPI:</span><span className="font-mono">Rp {selectedPayrollData.kpiBonus.toLocaleString('id-ID')}</span></div>
                    <div className="flex justify-between font-bold text-sm text-[#104480] pt-2 border-t border-sky-200">
                      <span>Total Gross:</span>
                      <span className="font-mono">Rp {selectedPayrollData.gross.toLocaleString('id-ID')}</span>
                    </div>
                  </div>

                  <div className="p-4 rounded-2xl bg-rose-50/60 border border-rose-200 space-y-2">
                    <h4 className="font-bold text-rose-900 border-b border-rose-200 pb-2">Potongan Absensi</h4>
                    <div className="flex justify-between"><span>Denda Keterlambatan ({selectedPayrollData.totalLateMins} m × Rp 800):</span><span className="font-mono text-rose-700">- Rp {selectedPayrollData.lateDeduction.toLocaleString('id-ID')}</span></div>
                    <div className="flex justify-between"><span>Potongan Izin Mendadak:</span><span className="font-mono text-rose-700">- Rp {selectedPayrollData.suddenDeduction.toLocaleString('id-ID')}</span></div>
                    <div className="flex justify-between"><span>Potongan Half-Day:</span><span className="font-mono text-rose-700">- Rp {selectedPayrollData.halfDayDeduction.toLocaleString('id-ID')}</span></div>
                    <div className="flex justify-between font-bold text-sm text-rose-900 pt-2 border-t border-rose-200">
                      <span>Total Potongan:</span>
                      <span className="font-mono">Rp {selectedPayrollData.totalDeduction.toLocaleString('id-ID')}</span>
                    </div>
                  </div>
                </div>

                <div className="bg-gradient-to-r from-[#07182e] via-[#0b2545] to-[#104480] text-white p-5 rounded-2xl flex flex-col sm:flex-row justify-between items-center gap-4">
                  <div>
                    <span className="text-xs font-bold uppercase text-sky-300">Take Home Pay (Gaji Bersih)</span>
                    <div className="text-2xl font-mono font-extrabold mt-0.5">
                      Rp {selectedPayrollData.netSalary.toLocaleString('id-ID')}
                    </div>
                  </div>
                  <button
                    onClick={() => setShowSlipModal(true)}
                    className="bg-white text-[#0b2545] hover:bg-sky-100 font-bold text-xs px-5 py-2.5 rounded-xl shadow flex items-center gap-1.5"
                  >
                    <Eye className="w-4 h-4" /> Lihat Slip Gaji Resmi
                  </button>
                </div>
              </div>
            )}

          </div>
        )}

      </main>

      {/* =================================================================== */}
      {/* MODALS FOR HRD MANAGEMENT                                           */}
      {/* =================================================================== */}

      {/* Modal 1: Edit Quote Penyemangat Depan */}
      {showQuoteModal && (
        <div className="fixed inset-0 bg-[#07182e]/60 backdrop-blur-sm z-50 flex items-center justify-center p-4">
          <div className="bg-white rounded-2xl max-w-md w-full p-6 shadow-2xl space-y-4">
            <h3 className="font-bold text-base text-[#0b2545]">Edit Kata-Kata Penyemangat (Interface Depan)</h3>
            <p className="text-xs text-slate-500">Teks ini akan tampil di halaman login awal dan banner motivasi karyawan secara live.</p>
            <textarea
              rows={3}
              value={tempQuote}
              onChange={(e) => setTempQuote(e.target.value)}
              className="w-full p-2.5 text-xs border rounded-xl focus:ring-2 focus:ring-[#104480]"
            />
            <div className="flex justify-end gap-2 pt-2 border-t text-xs">
              <button onClick={() => setShowQuoteModal(false)} className="px-3.5 py-1.5 border rounded-xl">Batal</button>
              <button
                onClick={() => {
                  setMotivationalQuote(tempQuote);
                  setShowQuoteModal(false);
                  showToast('Quote interface depan berhasil diperbarui!');
                }}
                className="px-4 py-1.5 bg-[#104480] text-white font-bold rounded-xl"
              >
                Simpan Quote
              </button>
            </div>
          </div>
        </div>
      )}

      {/* Modal 2: CRUD Edit / Tambah Karyawan */}
      {showEmpModal && (
        <div className="fixed inset-0 bg-[#07182e]/60 backdrop-blur-sm z-50 flex items-center justify-center p-4 overflow-y-auto">
          <form
            onSubmit={(e) => {
              e.preventDefault();
              if (editingEmpId) {
                setEmployees(employees.map(emp => emp.id === editingEmpId ? { ...emp, ...empForm } : emp));
                showToast(`Data karyawan ${empForm.name} diperbarui.`);
              } else {
                setEmployees([...employees, { ...empForm, userRole: 'Employee / Karyawan', email: `${empForm.id.toLowerCase()}@oasis.co.id` }]);
                showToast(`Karyawan baru ${empForm.name} berhasil ditambahkan.`);
              }
              setShowEmpModal(false);
            }}
            className="bg-white rounded-2xl max-w-lg w-full p-6 shadow-2xl space-y-4 text-xs"
          >
            <h3 className="font-bold text-base text-[#0b2545] border-b pb-2">
              {editingEmpId ? `Edit Master Data Karyawan (${editingEmpId})` : 'Tambah Karyawan Baru'}
            </h3>
            <div className="grid grid-cols-1 sm:grid-cols-2 gap-3">
              <div>
                <label className="block font-bold mb-1">ID Karyawan</label>
                <input
                  type="text"
                  value={empForm.id}
                  onChange={(e) => setEmpForm({ ...empForm, id: e.target.value })}
                  className="w-full p-2 border rounded-lg font-mono font-bold"
                  required
                />
              </div>
              <div>
                <label className="block font-bold mb-1">Nama Lengkap</label>
                <input
                  type="text"
                  value={empForm.name}
                  onChange={(e) => setEmpForm({ ...empForm, name: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                  required
                />
              </div>
              <div>
                <label className="block font-bold mb-1">Divisi / Departemen</label>
                <select
                  value={empForm.dept}
                  onChange={(e) => setEmpForm({ ...empForm, dept: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                >
                  {DIVISIONS.map(d => <option key={d} value={d}>{d}</option>)}
                </select>
              </div>
              <div>
                <label className="block font-bold mb-1">Jabatan</label>
                <input
                  type="text"
                  value={empForm.role}
                  onChange={(e) => setEmpForm({ ...empForm, role: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                  required
                />
              </div>
              <div>
                <label className="block font-bold mb-1">Nomor HP</label>
                <input
                  type="text"
                  value={empForm.phone}
                  onChange={(e) => setEmpForm({ ...empForm, phone: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                  required
                />
              </div>
              <div>
                <label className="block font-bold mb-1">Nomor Rekening Bank</label>
                <input
                  type="text"
                  value={empForm.bank}
                  onChange={(e) => setEmpForm({ ...empForm, bank: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                  required
                />
              </div>
              <div>
                <label className="block font-bold mb-1">Gaji Pokok (Rp)</label>
                <input
                  type="number"
                  value={empForm.baseSalary}
                  onChange={(e) => setEmpForm({ ...empForm, baseSalary: Number(e.target.value) })}
                  className="w-full p-2 border rounded-lg"
                />
              </div>
              <div>
                <label className="block font-bold mb-1">Password Akses Portal</label>
                <input
                  type="text"
                  value={empForm.password}
                  onChange={(e) => setEmpForm({ ...empForm, password: e.target.value })}
                  className="w-full p-2 border rounded-lg font-mono font-bold"
                  required
                />
              </div>
              <div className="sm:col-span-2">
                <label className="block font-bold mb-1">URL Foto Profil Karyawan</label>
                <input
                  type="text"
                  value={empForm.photo}
                  onChange={(e) => setEmpForm({ ...empForm, photo: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                />
              </div>
            </div>
            <div className="flex justify-end gap-2 pt-3 border-t">
              <button type="button" onClick={() => setShowEmpModal(false)} className="px-4 py-2 border rounded-xl">Batal</button>
              <button type="submit" className="px-4 py-2 bg-[#104480] text-white font-bold rounded-xl">Simpan Perubahan</button>
            </div>
          </form>
        </div>
      )}

      {/* Modal Konfirmasi Hapus Karyawan (Tanpa window.confirm) */}
      {confirmDeleteEmp && (
        <div className="fixed inset-0 bg-[#07182e]/60 backdrop-blur-sm z-50 flex items-center justify-center p-4">
          <div className="bg-white rounded-2xl max-w-sm w-full p-6 shadow-2xl space-y-4 text-xs">
            <h3 className="font-bold text-base text-rose-700">Konfirmasi Hapus Karyawan</h3>
            <p className="text-slate-600">
              Apakah Anda yakin ingin menghapus data karyawan <strong>{confirmDeleteEmp.name}</strong> ({confirmDeleteEmp.id}) dari sistem?
            </p>
            <div className="flex justify-end gap-2 pt-2 border-t">
              <button onClick={() => setConfirmDeleteEmp(null)} className="px-4 py-2 border rounded-xl font-bold">Batal</button>
              <button
                onClick={() => {
                  setEmployees(employees.filter(e => e.id !== confirmDeleteEmp.id));
                  showToast(`Karyawan ${confirmDeleteEmp.name} dihapus.`);
                  setConfirmDeleteEmp(null);
                }}
                className="px-4 py-2 bg-rose-600 text-white font-bold rounded-xl"
              >
                Ya, Hapus
              </button>
            </div>
          </div>
        </div>
      )}

      {/* Modal 3: Tambah / Edit Agenda Kalender HRD */}
      {showAgendaModal && (
        <div className="fixed inset-0 bg-[#07182e]/60 backdrop-blur-sm z-50 flex items-center justify-center p-4">
          <form
            onSubmit={(e) => {
              e.preventDefault();
              if (editingAgenda) {
                setHrdAgendas(hrdAgendas.map(a => a.id === editingAgenda.id ? { ...agendaForm, id: a.id } : a));
                showToast('Agenda rapat diperbarui.');
              } else {
                setHrdAgendas([...hrdAgendas, { ...agendaForm, id: `AGD-${Date.now()}` }]);
                showToast('Agenda rapat baru ditambahkan.');
              }
              setShowAgendaModal(false);
            }}
            className="bg-white rounded-2xl max-w-md w-full p-6 shadow-2xl space-y-4 text-xs"
          >
            <h3 className="font-bold text-base text-[#0b2545] border-b pb-2">
              {editingAgenda ? 'Edit Agenda Rapat / Koordinasi HRD' : 'Tambah Agenda Rapat HRD Baru'}
            </h3>
            <div className="space-y-3">
              <div>
                <label className="block font-bold mb-1">Judul Rapat / Agenda</label>
                <input
                  type="text"
                  value={agendaForm.title}
                  onChange={(e) => setAgendaForm({ ...agendaForm, title: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                  required
                />
              </div>
              <div className="grid grid-cols-3 gap-2">
                <div>
                  <label className="block font-bold mb-1">Tanggal</label>
                  <input
                    type="date"
                    value={agendaForm.date}
                    onChange={(e) => setAgendaForm({ ...agendaForm, date: e.target.value })}
                    className="w-full p-2 border rounded-lg"
                    required
                  />
                </div>
                <div>
                  <label className="block font-bold mb-1">Jam Mulai</label>
                  <input
                    type="time"
                    value={agendaForm.startTime}
                    onChange={(e) => setAgendaForm({ ...agendaForm, startTime: e.target.value })}
                    className="w-full p-2 border rounded-lg"
                    required
                  />
                </div>
                <div>
                  <label className="block font-bold mb-1">Jam Selesai</label>
                  <input
                    type="time"
                    value={agendaForm.endTime}
                    onChange={(e) => setAgendaForm({ ...agendaForm, endTime: e.target.value })}
                    className="w-full p-2 border rounded-lg"
                    required
                  />
                </div>
              </div>
              <div className="grid grid-cols-2 gap-2">
                <div>
                  <label className="block font-bold mb-1">Kategori</label>
                  <select
                    value={agendaForm.category}
                    onChange={(e) => setAgendaForm({ ...agendaForm, category: e.target.value })}
                    className="w-full p-2 border rounded-lg"
                  >
                    <option value="Koordinasi Internal">Koordinasi Internal</option>
                    <option value="Meeting Manajemen">Meeting Manajemen</option>
                    <option value="Interview & Rekrutmen">Interview & Rekrutmen</option>
                    <option value="Audit & Compliance">Audit & Compliance</option>
                  </select>
                </div>
                <div>
                  <label className="block font-bold mb-1">Lokasi / Ruang</label>
                  <input
                    type="text"
                    value={agendaForm.location}
                    onChange={(e) => setAgendaForm({ ...agendaForm, location: e.target.value })}
                    className="w-full p-2 border rounded-lg"
                  />
                </div>
              </div>
              <div>
                <label className="block font-bold mb-1">Deskripsi Kegiatan</label>
                <textarea
                  rows={2}
                  value={agendaForm.description}
                  onChange={(e) => setAgendaForm({ ...agendaForm, description: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                />
              </div>
            </div>
            <div className="flex justify-end gap-2 pt-2 border-t">
              <button type="button" onClick={() => setShowAgendaModal(false)} className="px-4 py-2 border rounded-xl">Batal</button>
              <button type="submit" className="px-4 py-2 bg-[#104480] text-white font-bold rounded-xl">Simpan Agenda</button>
            </div>
          </form>
        </div>
      )}

      {/* Modal 4: Tambah Kandidat Rekrutmen */}
      {showCandModal && (
        <div className="fixed inset-0 bg-[#07182e]/60 backdrop-blur-sm z-50 flex items-center justify-center p-4">
          <form
            onSubmit={(e) => {
              e.preventDefault();
              setCandidates([
                { id: `CND-${Date.now()}`, ...candForm, stage: 'Menunggu Evaluasi' },
                ...candidates
              ]);
              setShowCandModal(false);
              showToast('Kandidat baru berhasil ditambahkan.');
            }}
            className="bg-white rounded-2xl max-w-md w-full p-6 shadow-2xl space-y-4 text-xs"
          >
            <h3 className="font-bold text-base text-[#0b2545] border-b pb-2">Tambah Kandidat Interview & Skill Test</h3>
            <div className="space-y-3">
              <div>
                <label className="block font-bold mb-1">Nama Kandidat</label>
                <input
                  type="text"
                  value={candForm.name}
                  onChange={(e) => setCandForm({ ...candForm, name: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                  required
                />
              </div>
              <div className="grid grid-cols-2 gap-2">
                <div>
                  <label className="block font-bold mb-1">Posisi Dilamar</label>
                  <input
                    type="text"
                    value={candForm.position}
                    onChange={(e) => setCandForm({ ...candForm, position: e.target.value })}
                    className="w-full p-2 border rounded-lg"
                    required
                  />
                </div>
                <div>
                  <label className="block font-bold mb-1">Tanggal Interview</label>
                  <input
                    type="date"
                    value={candForm.interviewDate}
                    onChange={(e) => setCandForm({ ...candForm, interviewDate: e.target.value })}
                    className="w-full p-2 border rounded-lg"
                    required
                  />
                </div>
              </div>
              <div className="grid grid-cols-2 gap-2">
                <div>
                  <label className="block font-bold mb-1">Nilai Interview (0-100)</label>
                  <input
                    type="number"
                    value={candForm.interviewScore}
                    onChange={(e) => setCandForm({ ...candForm, interviewScore: Number(e.target.value) })}
                    className="w-full p-2 border rounded-lg"
                  />
                </div>
                <div>
                  <label className="block font-bold mb-1">Nilai Skill Test (0-100)</label>
                  <input
                    type="number"
                    value={candForm.skillTestScore}
                    onChange={(e) => setCandForm({ ...candForm, skillTestScore: Number(e.target.value) })}
                    className="w-full p-2 border rounded-lg"
                  />
                </div>
              </div>
              <div>
                <label className="block font-bold mb-1">Catatan Asesmen</label>
                <textarea
                  rows={2}
                  value={candForm.notes}
                  onChange={(e) => setCandForm({ ...candForm, notes: e.target.value })}
                  className="w-full p-2 border rounded-lg"
                />
              </div>
            </div>
            <div className="flex justify-end gap-2 pt-2 border-t">
              <button type="button" onClick={() => setShowCandModal(false)} className="px-4 py-2 border rounded-xl">Batal</button>
              <button type="submit" className="px-4 py-2 bg-[#104480] text-white font-bold rounded-xl">Simpan Kandidat</button>
            </div>
          </form>
        </div>
      )}

      {/* Modal 5: Override Jam Presensi HRD */}
      {overrideTarget && (
        <div className="fixed inset-0 bg-[#07182e]/60 backdrop-blur-sm z-50 flex items-center justify-center p-4">
          <div className="bg-white rounded-2xl max-w-sm w-full p-6 shadow-2xl space-y-4 text-xs">
            <h3 className="font-bold text-base text-[#0b2545]">Override Jam Presensi ({overrideTarget.empName})</h3>
            <div className="grid grid-cols-2 gap-3">
              <div>
                <label className="block font-bold mb-1">Jam Masuk (WIB)</label>
                <input
                  type="text"
                  value={overrideClockIn}
                  onChange={(e) => setOverrideClockIn(e.target.value)}
                  className="w-full p-2 border rounded-lg font-mono font-bold"
                />
              </div>
              <div>
                <label className="block font-bold mb-1">Jam Pulang (WIB)</label>
                <input
                  type="text"
                  value={overrideClockOut}
                  onChange={(e) => setOverrideClockOut(e.target.value)}
                  className="w-full p-2 border rounded-lg font-mono font-bold"
                />
              </div>
            </div>
            <div className="flex justify-end gap-2 pt-2 border-t">
              <button onClick={() => setOverrideTarget(null)} className="px-3 py-1.5 border rounded-xl">Batal</button>
              <button
                onClick={() => {
                  setRecords(
                    records.map(r =>
                      r.id === overrideTarget.id
                        ? { ...r, clockIn: overrideClockIn, clockOut: overrideClockOut, lateMinutes: 0, overrideByAdmin: true }
                        : r
                    )
                  );
                  setOverrideTarget(null);
                  showToast('Dispensasi / Override jam presensi disimpan.');
                }}
                className="px-4 py-1.5 bg-[#104480] text-white font-bold rounded-xl"
              >
                Simpan Override
              </button>
            </div>
          </div>
        </div>
      )}

      {/* Modal 6: Slip Gaji Resmi */}
      {showSlipModal && (
        <div className="fixed inset-0 bg-[#07182e]/70 backdrop-blur-sm z-50 flex items-center justify-center p-4">
          <div className="bg-white rounded-3xl max-w-lg w-full p-7 shadow-2xl space-y-5 text-xs">
            <div className="bg-gradient-to-r from-[#0b2545] to-[#104480] text-white p-4 rounded-2xl flex justify-between items-center">
              <OcrOasisLogo className="h-7" />
              <div className="text-right">
                <div className="font-extrabold">SLIP GAJI RESMI</div>
                <div className="text-[10px] text-sky-200 font-mono">NOVEMBER 2026</div>
              </div>
            </div>

            <div className="grid grid-cols-2 gap-2 bg-slate-50 p-3 rounded-xl border">
              <p><strong>Nama:</strong> {selectedPayrollData.emp.name}</p>
              <p><strong>ID:</strong> {selectedPayrollData.emp.id}</p>
              <p><strong>Divisi:</strong> {selectedPayrollData.emp.dept}</p>
              <p><strong>Rekening:</strong> {selectedPayrollData.emp.bank}</p>
            </div>

            <div className="space-y-1.5">
              <div className="flex justify-between"><span>Gaji Pokok + Tunjangan:</span><span className="font-mono">Rp {(selectedPayrollData.emp.baseSalary + selectedPayrollData.emp.allowances).toLocaleString('id-ID')}</span></div>
              <div className="flex justify-between"><span>Bonus Performance KPI:</span><span className="font-mono">Rp {selectedPayrollData.kpiBonus.toLocaleString('id-ID')}</span></div>
              <div className="flex justify-between text-rose-600"><span>Total Potongan Absensi:</span><span className="font-mono">- Rp {selectedPayrollData.totalDeduction.toLocaleString('id-ID')}</span></div>
              <div className="flex justify-between font-extrabold text-base text-[#0b2545] pt-2 border-t">
                <span>GAJI BERSIH DITERIMA:</span>
                <span className="font-mono">Rp {selectedPayrollData.netSalary.toLocaleString('id-ID')}</span>
              </div>
            </div>

            <div className="flex justify-end gap-2 pt-2 border-t">
              <button onClick={() => setShowSlipModal(false)} className="px-4 py-2 border rounded-xl font-bold">Tutup</button>
              <button
                onClick={() => {
                  window.print();
                  showToast('Dokumen Slip Gaji siap dicetak / disimpan PDF.');
                }}
                className="px-4 py-2 bg-[#104480] text-white font-bold rounded-xl flex items-center gap-1.5"
              >
                <Download className="w-3.5 h-3.5" /> Cetak / Unduh PDF
              </button>
            </div>
          </div>
        </div>
      )}

      {/* Footer */}
      <footer className="bg-white border-t border-slate-200 py-4 text-center text-xs text-slate-500">
        HRIS CV Oasis Creative Indonesia © 2026 • Integrated Corporate Operating System
      </footer>

    </div>
  );
}