<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Ride-Sharing App</title>
    <script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyBZf_PmUhFpWHBXxi2ygvHvOozMPXNOxFw&libraries=places,geometry"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif; }
        /* استخدام خط كايرو عند التحويل للعربية */
        [dir="rtl"] body { font-family: 'Cairo', sans-serif; }

        input[type="date"]::-webkit-datetime-edit-text,
        input[type="date"]::-webkit-datetime-edit-month-field,
        input[type="date"]::-webkit-datetime-edit-day-field,
        input[type="date"]::-webkit-datetime-edit-year-field { color: transparent; }
        input[type="date"]:focus::-webkit-datetime-edit-text,
        input[type="date"]:focus::-webkit-datetime-edit-month-field,
        input[type="date"]:focus::-webkit-datetime-edit-day-field,
        input[type="date"]:focus::-webkit-datetime-edit-year-field { color: white; }
        input[type="date"].has-value::-webkit-datetime-edit-text,
        input[type="date"].has-value::-webkit-datetime-edit-month-field,
        input[type="date"].has-value::-webkit-datetime-edit-day-field,
        input[type="date"].has-value::-webkit-datetime-edit-year-field { color: white; }

        @keyframes pulse-emergency {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: 0.8; transform: scale(1.02); }
        }
        .emergency-pulse { animation: pulse-emergency 1.5s infinite; }
        
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-5px); }
        }
        .car-float { animation: float 2s ease-in-out infinite; }
    </style>
</head>
<body>
    <div id="root"></div>
    <script type="text/babel">

let globalRideRequests = [];
let userProfiles = {
  'student@imamu.edu.sa': {
    name: 'Ahmed Student',
    email: 'student@imamu.edu.sa',
    studentId: '445012345',
    phone: '+966 50 123 4567',
    carModel: 'Toyota Camry 2022',
    carPlate: 'ABC-1234',
    joinedDate: '2024-01-15',
    walletBalance: 150,
    installments: [], 
    transactions: [
      { id: 1, type: 'deposit', amount: 200, date: '2024-12-01', description: 'Initial deposit' },
      { id: 2, type: 'payment', amount: -50, date: '2024-12-10', description: 'Trip payment' }
    ]
  }
};
let scheduledRides = [];

// --- TRANSLATION DICTIONARY ---
const translations = {
  en: {
    appTitle: 'Student Ride-Sharing App',
    appDescription: 'A simple and secure way for university students to coordinate rides, share costs, and commute to campus together.',
    overview: 'OVERVIEW',
    overviewText: 'The Student Ride-Sharing App provides a dedicated platform where verified students can register, log in, and manage shared rides.',
    vision: 'Vision: Build a trusted, safe, and efficient ride-sharing experience designed for university communities.',
    login: 'Login',
    register: 'Register',
    contactUs: 'CONTACT US',
    haveQuestion: 'Have a question?',
    name: 'Name',
    email: 'Email',
    message: 'Message',
    send: 'Send',
    welcomeBack: 'Welcome back',
    signInStudent: 'Please sign in with your student account.',
    loginAs: 'Login as',
    passenger: 'Passenger',
    driver: 'Driver',
    studentEmail: 'Student email',
    password: 'Password',
    forgotPassword: 'Forgot password?',
    logIn: 'Log in',
    noAccount: "Don't have an account?",
    createOne: 'Create one',
    passengerDashboard: 'PASSENGER DASHBOARD',
    driverDashboard: 'DRIVER DASHBOARD',
    passengerPanel: 'Passenger Panel',
    driverPanel: 'Driver Panel',
    wallet: 'Wallet',
    profile: 'Profile',
    history: 'History',
    viewMap: 'View Map',
    logout: 'Logout',
    requestNewRide: 'Request a New Ride',
    pickupLocation: 'Pickup Location',
    destination: 'Destination',
    numberOfPassengers: 'Number of Passengers',
    paymentMethod: 'Payment Method',
    cash: 'Cash',
    creditCard: 'Credit Card',
    requestNow: 'Request Now',
    schedule: 'Schedule',
    myRequests: 'My Requests',
    pending: 'Pending',
    accepted: 'Accepted',
    rejected: 'Rejected',
    from: 'From',
    to: 'To',
    passengers: 'Passengers',
    payment: 'Payment',
    driverInfo: 'Driver Information',
    chat: 'Chat',
    trackLive: 'Track Live',
    rate: 'Rate',
    trips: 'Trips',
    saved: 'SAR Saved',
    rating: 'Rating',
    sar: 'SAR',
    scheduledRides: 'Scheduled Rides',
    scheduled: 'Scheduled',
    cancelSchedule: 'Cancel Schedule',
    noRequests: 'No current requests',
    newRequests: 'New Requests',
    accept: 'Accept',
    reject: 'Reject',
    activeTrips: 'Active Trips',
    passengerContact: 'Passenger Contact',
    viewLocation: 'View Location',
    reviews: 'Reviews',
    myWallet: 'My Wallet',
    currentBalance: 'Current Balance',
    depositAmount: 'Deposit Amount',
    addMoney: 'Add Money',
    viewTransactions: 'View Transactions',
    transactionHistory: 'Transaction History',
    scheduleRide: 'Schedule Ride',
    date: 'Date',
    time: 'Time',
    repeat: 'Repeat',
    once: 'Once',
    daily: 'Daily',
    weekly: 'Weekly',
    weekdays: 'Weekdays Only',
    verificationCode: 'Verification Code',
    verify: 'Verify',
    editProfile: 'Edit Profile',
    save: 'Save',
    cancel: 'Cancel',
    memberSince: 'Member Since',
    tripHistory: 'Trip History',
    completed: 'Completed',
    back: 'Back',
    langBtn: 'العربية'
  },
  ar: {
    appTitle: 'تطبيق توصيل الطلاب',
    appDescription: 'طريقة بسيطة وآمنة لطلاب الجامعة لتنسيق الرحلات، مشاركة التكاليف، والوصول للجامعة معاً.',
    overview: 'نظرة عامة',
    overviewText: 'يوفر التطبيق منصة مخصصة حيث يمكن للطلاب الموثقين التسجيل وإدارة الرحلات المشتركة.',
    vision: 'الرؤية: بناء تجربة نقل موثوقة وآمنة وفعالة مصممة للمجتمعات الجامعية.',
    login: 'دخول',
    register: 'تسجيل',
    contactUs: 'تواصل معنا',
    haveQuestion: 'لديك استفسار؟',
    name: 'الاسم',
    email: 'البريد الإلكتروني',
    message: 'الرسالة',
    send: 'إرسال',
    welcomeBack: 'أهلاً بك مجدداً',
    signInStudent: 'يرجى تسجيل الدخول بحسابك الجامعي.',
    loginAs: 'تسجيل الدخول كـ',
    passenger: 'راكب',
    driver: 'سائق',
    studentEmail: 'البريد الجامعي',
    password: 'كلمة المرور',
    forgotPassword: 'نسيت كلمة المرور؟',
    logIn: 'تسجيل الدخول',
    noAccount: "ليس لديك حساب؟",
    createOne: 'أنشئ حساباً',
    passengerDashboard: 'لوحة الراكب',
    driverDashboard: 'لوحة السائق',
    passengerPanel: 'تحكم الراكب',
    driverPanel: 'تحكم السائق',
    wallet: 'المحفظة',
    profile: 'الملف الشخصي',
    history: 'السجل',
    viewMap: 'الخريطة',
    logout: 'خروج',
    requestNewRide: 'طلب رحلة جديدة',
    pickupLocation: 'موقع الانطلاق',
    destination: 'الوجهة',
    numberOfPassengers: 'عدد الركاب',
    paymentMethod: 'طريقة الدفع',
    cash: 'كاش',
    creditCard: 'بطاقة ائتمان',
    requestNow: 'اطلب الآن',
    schedule: 'جدولة',
    myRequests: 'طلباتي',
    pending: 'قيد الانتظار',
    accepted: 'مقبولة',
    rejected: 'مرفوضة',
    from: 'من',
    to: 'إلى',
    passengers: 'الركاب',
    payment: 'الدفع',
    driverInfo: 'معلومات السائق',
    chat: 'دردشة',
    trackLive: 'تتبع مباشر',
    rate: 'قيم',
    trips: 'رحلات',
    saved: 'ريال تم توفيره',
    rating: 'التقييم',
    sar: 'ريال',
    scheduledRides: 'الرحلات المجدولة',
    scheduled: 'مجدولة',
    cancelSchedule: 'إلغاء الجدولة',
    noRequests: 'لا توجد طلبات حالياً',
    newRequests: 'طلبات جديدة',
    accept: 'قبول',
    reject: 'رفض',
    activeTrips: 'رحلات نشطة',
    passengerContact: 'تواصل الراكب',
    viewLocation: 'عرض الموقع',
    reviews: 'التقييمات',
    myWallet: 'محفظتي',
    currentBalance: 'الرصيد الحالي',
    depositAmount: 'مبلغ الإيداع',
    addMoney: 'إضافة رصيد',
    viewTransactions: 'عرض العمليات',
    transactionHistory: 'سجل العمليات',
    scheduleRide: 'جدولة رحلة',
    date: 'التاريخ',
    time: 'الوقت',
    repeat: 'تكرار',
    once: 'مرة واحدة',
    daily: 'يومياً',
    weekly: 'أسبوعياً',
    weekdays: 'أيام الأسبوع فقط',
    verificationCode: 'رمز التحقق',
    verify: 'تحقق',
    editProfile: 'تعديل الملف',
    save: 'حفظ',
    cancel: 'إلغاء',
    memberSince: 'عضو منذ',
    tripHistory: 'سجل الرحلات',
    completed: 'مكتملة',
    back: 'عودة',
    langBtn: 'English'
  }
};

function App() {
  const [lang, setLang] = React.useState('en');
  const t = translations[lang]; // Auto-select text based on lang state

  // Effect to handle Direction (RTL/LTR)
  React.useEffect(() => {
    document.dir = lang === 'ar' ? 'rtl' : 'ltr';
  }, [lang]);

  const toggleLang = () => {
    setLang(prev => prev === 'en' ? 'ar' : 'en');
  };

  const [screen, setScreen] = React.useState('home');
  const [role, setRole] = React.useState('passenger');
  const [email, setEmail] = React.useState('');
  const [password, setPassword] = React.useState('');
  const [verificationCode, setVerificationCode] = React.useState('');
  const [generatedCode, setGeneratedCode] = React.useState('');
  const [pickupLocation, setPickupLocation] = React.useState('');
  const [destination, setDestination] = React.useState('');
  const [showNotification, setShowNotification] = React.useState(false);
  const [notificationMessage, setNotificationMessage] = React.useState('');
  const [notificationType, setNotificationType] = React.useState('success');
  const [refreshKey, setRefreshKey] = React.useState(0);
  const [showMap, setShowMap] = React.useState(false);
  
  // Refs
  const mapRef = React.useRef(null);
  const mapInstanceRef = React.useRef(null);
  const currentLocationMarkerRef = React.useRef(null);
  const destinationMarkerRef = React.useRef(null);
  const routePolylineRef = React.useRef(null);
  const pendingRouteRef = React.useRef(null);
  
  const [passengerCount, setPassengerCount] = React.useState(1);
  const [paymentMethod, setPaymentMethod] = React.useState('cash');
  const [currentLocation, setCurrentLocation] = React.useState(null);
  const [showRatingModal, setShowRatingModal] = React.useState(false);
  const [ratingData, setRatingData] = React.useState({ requestId: null, stars: 5, comment: '' });
  const [showReviewsModal, setShowReviewsModal] = React.useState(false);
  const [showTrackingModal, setShowTrackingModal] = React.useState(false);
  const [trackingData, setTrackingData] = React.useState(null);
  const trackingIntervalRef = React.useRef(null);
  const [showWalletModal, setShowWalletModal] = React.useState(false);
  const [depositAmount, setDepositAmount] = React.useState('');
  const [showTransactionsModal, setShowTransactionsModal] = React.useState(false);
  const [showInstallmentModal, setShowInstallmentModal] = React.useState(false);
  const [installmentCount, setInstallmentCount] = React.useState(2);
  const [currentInstallmentPrice, setCurrentInstallmentPrice] = React.useState(0);
  const [showInstallmentsListModal, setShowInstallmentsListModal] = React.useState(false);
  const [showEmergencyModal, setShowEmergencyModal] = React.useState(false);
  const [emergencyDescription, setEmergencyDescription] = React.useState('');
  const [currentEmergencyRequest, setCurrentEmergencyRequest] = React.useState(null);
  const [showScheduleModal, setShowScheduleModal] = React.useState(false);
  const [scheduleDate, setScheduleDate] = React.useState('');
  const [scheduleTime, setScheduleTime] = React.useState('');
  const [scheduleRecurring, setScheduleRecurring] = React.useState('once');
  const [showChat, setShowChat] = React.useState(false);
  const [chatMessages, setChatMessages] = React.useState([{ id: 1, sender: 'driver', text: 'Hello! I am on my way', time: '10:30' }]);
  const [newMessage, setNewMessage] = React.useState('');
  const [currentChatWith, setCurrentChatWith] = React.useState('');
  const [isEditing, setIsEditing] = React.useState(false);
  const [editedProfile, setEditedProfile] = React.useState({
    name: userProfiles[email]?.name || 'Ahmed Student',
    phone: userProfiles[email]?.phone || '+966 50 123 4567',
    studentId: userProfiles[email]?.studentId || '445012345',
    carModel: userProfiles[email]?.carModel || 'Toyota Camry 2022',
    carPlate: userProfiles[email]?.carPlate || 'ABC-1234'
  });

  const handleSaveProfile = () => {
    userProfiles[email] = { ...userProfiles[email], ...editedProfile, email: email, joinedDate: userProfiles[email]?.joinedDate || '2024-01-15' };
    setIsEditing(false);
    showNotif('✅ Profile updated successfully', 'success');
  };

  const handleLogout = () => {
    setScreen('home');
    setShowMap(false);
    setRole('passenger');
    pendingRouteRef.current = null;
  };

  // Auto-detect completed rides for rating
  React.useEffect(() => {
    if (role === 'passenger' && email) {
        const unratedRide = globalRideRequests.find(r => 
            r.passenger === email && 
            (r.completed || r.tripStatus === 'completed') && 
            !r.rating
        );
        if (unratedRide) {
            setRatingData({ requestId: unratedRide.id, stars: 5, comment: '' });
            setShowRatingModal(true);
        }
    }
  }, [role, email, refreshKey, screen]);

  // Auto-deduction
  React.useEffect(() => {
    const installmentInterval = setInterval(() => {
        if (userProfiles[email]?.installments) {
        const now = new Date();
        userProfiles[email].installments.forEach((installment) => {
            if (installment.status === 'pending' && new Date(installment.dueDate) <= now) {
            const balance = userProfiles[email].walletBalance || 0;
            if (balance >= installment.amount) {
                userProfiles[email].walletBalance -= installment.amount;
                installment.status = 'paid';
                installment.paidDate = now.toISOString();
                userProfiles[email].transactions.unshift({ id: Date.now(), type: 'installment', amount: -installment.amount, date: now.toLocaleDateString('en-US'), description: `Split Payment ${installment.installmentNumber}/${installment.totalInstallments}` });
                showNotif(`💳 Split ${installment.amount} SAR deducted from wallet`, 'success');
                setRefreshKey(prev => prev + 1);
            }
            }
        });
        }
    }, 10000); 
    return () => clearInterval(installmentInterval);
    }, [email]);

  React.useEffect(() => {
    if (navigator.geolocation) {
      navigator.geolocation.getCurrentPosition(
        (position) => {
          const location = { lat: position.coords.latitude, lng: position.coords.longitude };
          setCurrentLocation(location);
          const geocoder = new google.maps.Geocoder();
          geocoder.geocode({ location: location }, (results, status) => {
            if (status === 'OK' && results[0]) setPickupLocation(results[0].formatted_address);
          });
        },
        (error) => { setCurrentLocation({ lat: 24.7136, lng: 46.6753 }); }
      );
    }
  }, []);

  React.useEffect(() => {
    if (showMap && mapRef.current) {
      const center = currentLocation || { lat: 24.7136, lng: 46.6753 };
      mapInstanceRef.current = new google.maps.Map(mapRef.current, { center: center, zoom: 13, styles: [ { "featureType": "all", "elementType": "geometry", "stylers": [{"color": "#242f3e"}] }, { "featureType": "all", "elementType": "labels.text.stroke", "stylers": [{"lightness": -80}] }, { "featureType": "administrative", "elementType": "labels.text.fill", "stylers": [{"color": "#746855"}] }, { "featureType": "poi", "elementType": "labels.text.fill", "stylers": [{"color": "#d59563"}] }, { "featureType": "road", "elementType": "geometry.fill", "stylers": [{"color": "#2b3544"}] }, { "featureType": "road", "elementType": "labels.text.fill", "stylers": [{"color": "#9ca5b3"}] }, { "featureType": "water", "elementType": "geometry", "stylers": [{"color": "#17263c"}] } ] });
      if (currentLocation) {
        currentLocationMarkerRef.current = new google.maps.Marker({ position: currentLocation, map: mapInstanceRef.current, title: "Your Location", icon: { path: google.maps.SymbolPath.CIRCLE, scale: 10, fillColor: "#10b981", fillOpacity: 1, strokeWeight: 2, strokeColor: "#ffffff" } });
      }
      if (pendingRouteRef.current && currentLocation) {
        drawRoute(currentLocation, pendingRouteRef.current);
        pendingRouteRef.current = null;
      }
    }
  }, [showMap]);

  const drawRoute = (start, end) => {
    if (!mapInstanceRef.current) return;
    const directionsService = new google.maps.DirectionsService();
    directionsService.route( { origin: start, destination: end, travelMode: google.maps.TravelMode.DRIVING }, (result, status) => { if (status === google.maps.DirectionsStatus.OK) { if (routePolylineRef.current) routePolylineRef.current.setMap(null); const path = result.routes[0].overview_path; routePolylineRef.current = new google.maps.Polyline({ path: path, geodesic: true, strokeColor: '#10b981', strokeOpacity: 1.0, strokeWeight: 4, map: mapInstanceRef.current }); if (destinationMarkerRef.current) destinationMarkerRef.current.setMap(null); destinationMarkerRef.current = new google.maps.Marker({ position: end, map: mapInstanceRef.current, title: "Destination", icon: { path: google.maps.SymbolPath.CIRCLE, scale: 10, fillColor: "#ef4444", fillOpacity: 1, strokeWeight: 2, strokeColor: "#ffffff" } }); const bounds = new google.maps.LatLngBounds(); path.forEach(point => bounds.extend(point)); mapInstanceRef.current.fitBounds(bounds); const route = result.routes[0]; showNotif(`📍 Distance: ${route.legs[0].distance.text} | ⏱️ Time: ${route.legs[0].duration.text}`, 'success'); } });
  };

  const showNotif = (message, type = 'success') => {
    setNotificationMessage(message); setNotificationType(type); setShowNotification(true);
    setTimeout(() => setShowNotification(false), 3000);
  };

  const handleLogin = () => {
    if (!email.endsWith('@imamu.edu.sa')) { showNotif('⚠️ Use university email', 'error'); return; }
    if (password.length < 8) { showNotif('⚠️ Password must be 8+ characters', 'error'); return; }
    const code = Math.floor(100000 + Math.random() * 900000).toString();
    setGeneratedCode(code); showNotif(`📧 Verification code sent: ${code}`, 'success'); setScreen('verification');
  };

  const handleVerification = () => {
    if (verificationCode === generatedCode) { showNotif('✅ Verification successful', 'success'); setTimeout(() => { setScreen(role === 'driver' ? 'driver' : 'passenger'); }, 800); } else { showNotif('⚠️ Invalid verification code', 'error'); }
  };

  const handleDeposit = () => {
    const amount = parseFloat(depositAmount);
    if (isNaN(amount) || amount <= 0) { showNotif('⚠️ Enter a valid amount', 'error'); return; }
    if (!userProfiles[email]) userProfiles[email] = { walletBalance: 0, transactions: [] };
    userProfiles[email].walletBalance = (userProfiles[email].walletBalance || 0) + amount;
    userProfiles[email].transactions = userProfiles[email].transactions || [];
    userProfiles[email].transactions.unshift({ id: Date.now(), type: 'deposit', amount: amount, date: new Date().toLocaleDateString('en-US'), description: 'Wallet deposit' });
    showNotif(`✅ ${amount} SAR added to wallet`, 'success'); setDepositAmount(''); setShowWalletModal(false); setRefreshKey(prev => prev + 1);
  };

  const handleInstallmentPayment = () => {
    const price = currentInstallmentPrice || Math.floor(Math.random() * 20) + 10;
    const firstPayment = parseFloat((price / installmentCount).toFixed(2));
    const balance = userProfiles[email]?.walletBalance || 0;
    if (balance < firstPayment) { showNotif('⚠️ Insufficient balance for first Split payment', 'error'); return; }
    userProfiles[email].walletBalance -= firstPayment;
    userProfiles[email].transactions.unshift({ id: Date.now(), type: 'installment', amount: -firstPayment, date: new Date().toLocaleDateString('en-US'), description: `First Split (1/${installmentCount})` });
    if (!userProfiles[email].installments) userProfiles[email].installments = [];
    const now = new Date();
    for (let i = 2; i <= installmentCount; i++) {
        const dueDate = new Date(now);
        dueDate.setSeconds(dueDate.getSeconds() + (i - 1) * 10); 
        userProfiles[email].installments.push({ id: Date.now() + i, installmentNumber: i, totalInstallments: installmentCount, amount: firstPayment, dueDate: dueDate.toISOString(), status: 'pending', tripDescription: `${pickupLocation} to ${destination}`, createdDate: now.toISOString() });
    }
    const newRequest = { id: Date.now(), passenger: email, passengerName: userProfiles[email]?.name || 'Ahmed Student', from: pickupLocation, to: destination, paymentMethod: 'installment', passengerCount: passengerCount, installmentInfo: { total: installmentCount, paid: 1, remaining: installmentCount - 1, amountPerInstallment: firstPayment }, time: new Date().toLocaleTimeString('en-US', {hour: '2-digit', minute: '2-digit'}), date: new Date().toLocaleDateString('en-US'), status: 'pending', driverInfo: null, price: price, rating: null, reviews: [], completed: false };
    globalRideRequests.push(newRequest);
    showNotif(`✅ First Split ${firstPayment} SAR deducted. ${installmentCount - 1} remaining`, 'success');
    setShowInstallmentModal(false); setShowWalletModal(false); setPickupLocation(''); setDestination(''); setRefreshKey(prev => prev + 1);
  };

  const handleEmergencyAlert = () => {
    if (!emergencyDescription.trim()) { showNotif('⚠️ Please describe the emergency', 'error'); return; }
    const alert = { id: Date.now(), requestId: currentEmergencyRequest.id, passenger: email, passengerName: userProfiles[email]?.name || 'Ahmed Student', description: emergencyDescription, location: currentLocation, timestamp: new Date().toISOString(), status: 'active', tripDetails: { from: currentEmergencyRequest.from, to: currentEmergencyRequest.to, driverInfo: currentEmergencyRequest.driverInfo } };
    emergencyAlerts.push(alert); currentEmergencyRequest.emergencyReported = true; showNotif('🚨 Emergency alert sent! Help is on the way', 'error'); setShowEmergencyModal(false); setEmergencyDescription(''); setRefreshKey(prev => prev + 1);
  };

  const handleScheduleRide = () => {
    if (!pickupLocation || !destination || !scheduleDate || !scheduleTime) { showNotif('⚠️ Fill all schedule details', 'error'); return; }
    const scheduledRide = { id: Date.now(), passenger: email, passengerName: userProfiles[email]?.name || 'Ahmed Student', from: pickupLocation, to: destination, passengerCount: passengerCount, paymentMethod: paymentMethod, scheduleDate: scheduleDate, scheduleTime: scheduleTime, recurring: scheduleRecurring, status: 'scheduled', price: Math.floor(Math.random() * 20) + 10 };
    scheduledRides.push(scheduledRide); showNotif('📅 Ride scheduled successfully', 'success'); setShowScheduleModal(false); setPickupLocation(''); setDestination(''); setScheduleDate(''); setScheduleTime(''); setScheduleRecurring('once'); setRefreshKey(prev => prev + 1);
  };

  const requestRide = () => {
    if (!pickupLocation || !destination) { showNotif('⚠️ Enter location and destination', 'error'); return; }
    const price = Math.floor(Math.random() * 20) + 10;
    if (paymentMethod === 'installment') { setCurrentInstallmentPrice(price); setShowInstallmentModal(true); return; }
    if (paymentMethod === 'wallet') {
      const balance = userProfiles[email]?.walletBalance || 0;
      if (balance < price) { showNotif('⚠️ Insufficient wallet balance', 'error'); setShowWalletModal(true); return; }
    }
    const newRequest = { id: Date.now(), passenger: email || 'Passenger', passengerName: userProfiles[email]?.name || 'Ahmed Student', passengerRating: '4.9', from: pickupLocation, to: destination, passengerCount: passengerCount, paymentMethod: paymentMethod, time: new Date().toLocaleTimeString('en-US', {hour: '2-digit', minute: '2-digit'}), date: new Date().toLocaleDateString('en-US'), status: 'pending', driverInfo: null, price: price, rating: null, reviews: [], completed: false };
    globalRideRequests.push(newRequest);
    if (paymentMethod === 'wallet') { userProfiles[email].walletBalance -= price; userProfiles[email].transactions.unshift({ id: Date.now(), type: 'payment', amount: -price, date: new Date().toLocaleDateString('en-US'), description: `Trip payment - ${pickupLocation} to ${destination}` }); }
    showNotif('📤 Request sent successfully', 'success');
    
    if (currentLocation && destination) { 
        const geocoder = new google.maps.Geocoder(); 
        geocoder.geocode({ address: destination }, (results, status) => { 
            if (status === 'OK') { 
                pendingRouteRef.current = results[0].geometry.location; 
                setShowMap(true); 
            } 
        }); 
    } else {
        setShowMap(true); 
    }
    setPickupLocation(''); setDestination(''); setPassengerCount(1); setPaymentMethod('cash'); setRefreshKey(prev => prev + 1);
  };

  const openChat = (withPerson) => { setCurrentChatWith(withPerson); setShowChat(true); };
  const sendMessage = () => { if (newMessage.trim()) { const msg = { id: Date.now(), sender: role === 'driver' ? 'driver' : 'passenger', text: newMessage, time: new Date().toLocaleTimeString('en-US', {hour: '2-digit', minute: '2-digit'}) }; setChatMessages(prev => [...prev, msg]); setNewMessage(''); if (role === 'passenger') { setTimeout(() => { const reply = { id: Date.now()+1, sender: 'driver', text: 'Ok, got it. I will be there soon.', time: new Date().toLocaleTimeString('en-US', {hour: '2-digit', minute: '2-digit'}) }; setChatMessages(prev => [...prev, reply]); }, 3000); } } };

  const submitRating = () => {
    const request = globalRideRequests.find(r => r.id === ratingData.requestId);
    if (request) {
      const review = { id: Date.now(), stars: ratingData.stars, comment: ratingData.comment, date: new Date().toLocaleDateString('en-US'), passengerName: request.passengerName };
      if (!request.reviews) request.reviews = [];
      request.reviews.push(review);
      request.rating = ratingData.stars;
      showNotif('⭐ Rating submitted successfully', 'success');
      setShowRatingModal(false);
      setRefreshKey(prev => prev + 1);
    }
  };

  // --- FIX FOR LIVE TRACKING ---
  const startLiveTracking = (request) => {
    // 1. Force close other blocking modals
    setShowMap(false);
    setShowWalletModal(false);
    
    // 2. Set Tracking Data (Use fallback location if GPS is slow)
    setTrackingData({
      requestId: request.id,
      driverLocation: currentLocation || { lat: 24.7136, lng: 46.6753 }, // Fallback
      destination: { lat: 24.7136 + 0.02, lng: 46.6753 + 0.02 },
      status: 'on_way',
      eta: 8,
      speed: 45,
      distance: 3.2
    });

    // 3. Show Modal
    setShowTrackingModal(true);

    // 4. Start Interval
    if (trackingIntervalRef.current) clearInterval(trackingIntervalRef.current);
    trackingIntervalRef.current = setInterval(() => {
      setTrackingData(prev => {
        if (!prev) return null;
        const newDistance = Math.max(0, prev.distance - 0.1);
        const newEta = Math.max(0, prev.eta - 0.2);
        return { 
            ...prev, 
            distance: newDistance, 
            eta: newEta, 
            speed: 40 + Math.random() * 5, 
            status: newDistance <= 0.1 ? 'arrived' : 'on_way' 
        };
      });
    }, 2000);
  };

  const closeTracking = () => { if (trackingIntervalRef.current) clearInterval(trackingIntervalRef.current); setShowTrackingModal(false); setTrackingData(null); };

  // --- LANGUAGE SWITCH BUTTON COMPONENT ---
  const LangButton = () => (
      <button 
          onClick={toggleLang}
          className="fixed top-6 left-6 z-50 bg-white/20 backdrop-blur-md border border-white/30 text-white px-4 py-2 rounded-full font-bold shadow-lg hover:bg-white/30 transition flex items-center gap-2"
          style={{direction: 'ltr'}} // Keep button text LTR
      >
          🌐 {t.langBtn}
      </button>
  );

  if (screen === 'verification') { return (<div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black flex items-center justify-center p-6"><LangButton/>{showNotification && (<div className={`fixed top-6 right-6 px-6 py-3 rounded-lg shadow-lg z-50 ${notificationType === 'success' ? 'bg-green-500' : 'bg-red-500'} text-white font-medium`}>{notificationMessage}</div>)}<div className="w-full max-w-md"><div className="bg-slate-900/90 backdrop-blur-xl rounded-2xl p-8 border border-white/10 shadow-2xl"><div className="text-center mb-8"><div className="text-6xl mb-4">🔐</div><h2 className="text-3xl font-bold text-white mb-2">{t.verificationCode}</h2><p className="text-white/60">Enter the code sent to your email</p><p className="text-green-400 text-sm mt-2">{email}</p></div><div className="space-y-4"><div><label className="text-white/80 text-sm block mb-2">{t.verificationCode}</label><input type="text" placeholder="000000" maxLength="6" value={verificationCode} onChange={(e) => setVerificationCode(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white text-center text-2xl tracking-widest placeholder-white/40 focus:outline-none focus:border-blue-400 transition" /></div><button onClick={handleVerification} className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg transition shadow-lg">{t.verify}</button><button onClick={() => setScreen('login')} className="w-full text-blue-400 hover:text-blue-300 text-sm transition">← {t.back}</button></div><div className="mt-6 pt-6 border-t border-white/10 text-center"><p className="text-white/40 text-xs">Demo code: {generatedCode}</p></div></div></div></div>); }
  if (screen === 'profile') { const profile = userProfiles[email] || {}; return (<div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black pb-12"><LangButton/>{showNotification && (<div className={`fixed top-6 right-6 px-6 py-3 rounded-lg shadow-lg z-50 ${notificationType === 'success' ? 'bg-green-500' : 'bg-red-500'} text-white font-medium`}>{notificationMessage}</div>)}<div className="container mx-auto px-6 py-8"><div className="flex items-center justify-between mb-8"><h1 className="text-4xl font-bold text-white">👤 {t.profile}</h1><div className="flex gap-3">{isEditing ? (<><button onClick={handleSaveProfile} className="bg-green-500 hover:bg-green-600 text-white px-6 py-2.5 rounded-lg font-semibold">💾 {t.save}</button><button onClick={() => { setIsEditing(false); setEditedProfile({ name: profile.name || 'User Name', phone: profile.phone || '+966 50 123 4567', studentId: profile.studentId || '445012345', carModel: profile.carModel || 'Toyota Camry 2022', carPlate: profile.carPlate || 'ABC-1234' }); }} className="bg-red-500 hover:bg-red-600 text-white px-6 py-2.5 rounded-lg font-semibold">✕ {t.cancel}</button></>) : (<button onClick={() => setIsEditing(true)} className="bg-blue-500 hover:bg-blue-600 text-white px-6 py-2.5 rounded-lg font-semibold">✏️ {t.editProfile}</button>)}<button onClick={() => setScreen(role === 'driver' ? 'driver' : 'passenger')} className="bg-slate-800/50 hover:bg-slate-800 text-white px-6 py-2.5 rounded-lg border border-white/10">← {t.back}</button></div></div><div className="max-w-3xl mx-auto"><div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-8 border border-white/10 mb-6"><div className="flex items-center gap-6 mb-8"><div className="w-24 h-24 rounded-full bg-gradient-to-br from-green-400 to-blue-600 flex items-center justify-center text-4xl">{role === 'driver' ? '🚗' : '🎒'}</div><div className="flex-1">{isEditing ? (<input type="text" value={editedProfile.name} onChange={(e) => setEditedProfile({...editedProfile, name: e.target.value})} className="w-full text-3xl font-bold text-white bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2 focus:outline-none focus:border-blue-400" />) : (<h2 className="text-3xl font-bold text-white">{editedProfile.name}</h2>)}<p className="text-white/60 mt-2">{role === 'driver' ? t.driver : t.passenger}</p></div></div><div className="space-y-4"><div className="flex items-center gap-4 p-4 bg-slate-800/50 rounded-lg"><span className="text-2xl">📧</span><div className="flex-1"><p className="text-white/60 text-sm">{t.email}</p><p className="text-white">{email}</p></div></div><div className="flex items-center gap-4 p-4 bg-slate-800/50 rounded-lg"><span className="text-2xl">🎓</span><div className="flex-1"><p className="text-white/60 text-sm">Student ID</p>{isEditing ? (<input type="text" value={editedProfile.studentId} onChange={(e) => setEditedProfile({...editedProfile, studentId: e.target.value})} className="w-full text-white bg-slate-700/50 border border-blue-500/30 rounded-lg px-3 py-1.5 mt-1 focus:outline-none focus:border-blue-400" />) : (<p className="text-white">{editedProfile.studentId}</p>)}</div></div><div className="flex items-center gap-4 p-4 bg-slate-800/50 rounded-lg"><span className="text-2xl">📱</span><div className="flex-1"><p className="text-white/60 text-sm">Phone</p>{isEditing ? (<input type="text" value={editedProfile.phone} onChange={(e) => setEditedProfile({...editedProfile, phone: e.target.value})} className="w-full text-white bg-slate-700/50 border border-blue-500/30 rounded-lg px-3 py-1.5 mt-1 focus:outline-none focus:border-blue-400" />) : (<p className="text-white">{editedProfile.phone}</p>)}</div></div>{role === 'driver' && (<><div className="flex items-center gap-4 p-4 bg-slate-800/50 rounded-lg"><span className="text-2xl">🚙</span><div className="flex-1"><p className="text-white/60 text-sm">Car Model</p>{isEditing ? (<input type="text" value={editedProfile.carModel} onChange={(e) => setEditedProfile({...editedProfile, carModel: e.target.value})} className="w-full text-white bg-slate-700/50 border border-blue-500/30 rounded-lg px-3 py-1.5 mt-1 focus:outline-none focus:border-blue-400" />) : (<p className="text-white">{editedProfile.carModel}</p>)}</div></div><div className="flex items-center gap-4 p-4 bg-slate-800/50 rounded-lg"><span className="text-2xl">🔢</span><div className="flex-1"><p className="text-white/60 text-sm">Plate Number</p>{isEditing ? (<input type="text" value={editedProfile.carPlate} onChange={(e) => setEditedProfile({...editedProfile, carPlate: e.target.value})} className="w-full text-white bg-slate-700/50 border border-blue-500/30 rounded-lg px-3 py-1.5 mt-1 focus:outline-none focus:border-blue-400" />) : (<p className="text-white">{editedProfile.carPlate}</p>)}</div></div></>)}<div className="flex items-center gap-4 p-4 bg-slate-800/50 rounded-lg"><span className="text-2xl">📅</span><div><p className="text-white/60 text-sm">{t.memberSince}</p><p className="text-white">{profile.joinedDate || '2024-01-15'}</p></div></div></div></div></div></div></div>); }

  if (screen === 'history') {
    const completedRides = globalRideRequests.filter(r => {
        const isCompleted = r.tripStatus === 'completed' || r.completed;
        const isMyRole = (role === 'driver' || r.passenger === email);
        if (role === 'driver') return isCompleted && isMyRole;
        else return isCompleted && isMyRole && r.rating;
    });

    return (
      <div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black pb-12">
        <LangButton/>
        <div className="container mx-auto px-6 py-8">
          <div className="flex items-center justify-between mb-8"><h1 className="text-4xl font-bold text-white">📜 {t.tripHistory}</h1><button onClick={() => setScreen(role === 'driver' ? 'driver' : 'passenger')} className="bg-slate-800/50 hover:bg-slate-800 text-white px-6 py-2.5 rounded-lg border border-white/10">← {t.back}</button></div>
          {completedRides.length > 0 ? (
            <div className="space-y-4">{completedRides.map((ride) => (<div key={ride.id} className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10"><div className="flex justify-between items-start mb-4"><div><div className="inline-block px-3 py-1 rounded-full text-sm font-medium mb-2 bg-green-500/20 text-green-400">✅ {t.completed}</div><p className="text-white/60 text-sm">{ride.date} - {ride.time}</p></div><div className="text-right"><p className="text-2xl font-bold text-green-400">{ride.price} {t.sar}</p></div></div><div className="bg-slate-800/50 rounded-lg p-4 mb-4"><p className="text-white mb-2">📍 {t.from}: {ride.from}</p><p className="text-white mb-2">🎯 {t.to}: {ride.to}</p><div className="flex gap-4 mt-3 pt-3 border-t border-white/10"><p className="text-white/80 text-sm">👥 {t.passengers}: <span className="text-green-400 font-semibold">{ride.passengerCount}</span></p><p className="text-white/80 text-sm">💳 {t.payment}: <span className="text-blue-400 font-semibold">{ride.paymentMethod === 'cash' ? t.cash : ride.paymentMethod === 'card' ? t.creditCard : ride.paymentMethod === 'installment' ? 'Split' : t.wallet}</span></p></div></div>{role === 'driver' ? (<div className="bg-blue-500/10 border border-blue-500/30 rounded-lg p-4"><p className="text-white font-semibold mb-2">👤 {t.passenger}: {ride.passengerName}</p><p className="text-white/80 text-sm">📧 {ride.passenger}</p>{ride.rating && (<p className="text-yellow-400 text-sm mt-2">⭐ {t.rating}: {'⭐'.repeat(ride.rating)}</p>)}</div>) : (ride.driverInfo && (<div className="bg-green-500/10 border border-green-500/30 rounded-lg p-4"><p className="text-white font-semibold mb-2">🚗 {t.driver}: {ride.driverInfo.name}</p><p className="text-yellow-400 text-sm">⭐ {ride.driverInfo.rating} ({ride.driverInfo.rides} {t.trips})</p></div>))}</div>))}</div>
          ) : (<div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-12 border border-white/10 text-center"><p className="text-6xl mb-4">📭</p><p className="text-white/60">No completed trips yet</p></div>)}
        </div>
      </div>
    );
  }

  // Home, Login... (Keep same)
  if (screen === 'home') {
    return (
      <div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black flex items-center justify-center p-6">
        <LangButton/>
        <div className="w-full max-w-6xl flex flex-col lg:flex-row gap-8 items-start"><div className="flex-1 text-white"><h1 className="text-5xl font-bold mb-4">{t.appTitle}</h1><p className="text-lg mb-8 text-white/80">{t.appDescription}</p><div className="mb-8"><h3 className="text-xl font-semibold mb-3 text-blue-300">{t.overview}</h3><p className="text-white/70 mb-4">{t.overviewText}</p><p className="text-blue-200 italic">{t.vision}</p></div><div className="flex gap-4 flex-wrap"><button onClick={() => setScreen('login')} className="px-8 py-3 bg-white text-blue-600 rounded-full font-semibold hover:bg-blue-50 transition">{t.login}</button><button onClick={() => setScreen('register')} className="px-8 py-3 bg-blue-600/30 backdrop-blur-sm text-white rounded-full font-semibold border border-white/30 hover:bg-blue-600/50 transition">{t.register}</button></div></div><div className="w-full lg:w-96"><div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10"><h3 className="text-white font-semibold mb-2">{t.contactUs}</h3><p className="text-white/60 text-sm mb-4">{t.haveQuestion}</p><div className="space-y-4"><div><label className="text-white/80 text-sm block mb-2">{t.name}</label><input type="text" placeholder={t.name} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2.5 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div><div><label className="text-white/80 text-sm block mb-2">{t.email}</label><input type="email" placeholder="you@example.com" className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2.5 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div><div><label className="text-white/80 text-sm block mb-2">{t.message}</label><textarea placeholder={t.message} rows="3" className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2.5 text-white placeholder-white/40 focus:outline-none focus:border-blue-400 resize-none"></textarea></div><button className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-2.5 rounded-lg transition">{t.send}</button></div></div></div></div>
      </div>
    );
  }
  if (screen === 'login') {
    return (
      <div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black flex items-center justify-center p-6">
        <LangButton/>
        {showNotification && (<div className={`fixed top-6 right-6 px-6 py-3 rounded-lg shadow-lg z-50 ${notificationType === 'success' ? 'bg-green-500' : 'bg-red-500'} text-white font-medium`}>{notificationMessage}</div>)}
        <div className="w-full max-w-md"><div className="bg-slate-900/90 backdrop-blur-xl rounded-2xl p-8 border border-white/10 shadow-2xl"><div className="mb-6"><div className="inline-flex items-center gap-2 bg-green-500/20 backdrop-blur-sm px-3 py-1.5 rounded-full mb-4"><span className="w-2 h-2 bg-green-400 rounded-full"></span><span className="text-green-300 text-xs font-medium">STUDENT RIDE-SHARING PLATFORM</span></div><h2 className="text-3xl font-bold text-white mb-2">{t.welcomeBack}</h2><p className="text-white/60">{t.signInStudent}</p></div><div className="mb-4"><label className="text-white/80 text-sm block mb-2">{t.loginAs}</label><div className="flex gap-3"><button onClick={() => setRole('passenger')} className={`flex-1 py-2.5 rounded-lg font-medium transition ${role === 'passenger' ? 'bg-green-500 text-white' : 'bg-slate-800/50 text-white/60 hover:bg-slate-800'}`}>🧑 {t.passenger}</button><button onClick={() => setRole('driver')} className={`flex-1 py-2.5 rounded-lg font-medium transition ${role === 'driver' ? 'bg-green-500 text-white' : 'bg-slate-800/50 text-white/60 hover:bg-slate-800'}`}>🚗 {t.driver}</button></div></div><div className="space-y-4"><div><label className="text-white/80 text-sm block mb-2">{t.studentEmail}</label><input type="email" placeholder="you@imamu.edu.sa" value={email} onChange={(e) => setEmail(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400 transition" /></div><div><label className="text-white/80 text-sm block mb-2">{t.password}</label><input type="password" placeholder="••••••••" value={password} onChange={(e) => setPassword(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400 transition" /><div className="text-right mt-2"><button onClick={() => setScreen('forgot')} className="text-blue-400 text-sm hover:text-blue-300 transition">{t.forgotPassword}</button></div></div><button onClick={handleLogin} className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg transition shadow-lg">{t.logIn}</button><p className="text-center text-white/60 text-sm">{t.noAccount}{' '}<button onClick={() => setScreen('register')} className="text-blue-400 hover:text-blue-300 transition">{t.createOne}</button></p></div><div className="mt-6 pt-6 border-t border-white/10"><p className="text-white/40 text-xs text-center">Demo: student@imamu.edu.sa / password123</p></div></div><div className="text-center mt-6"><button onClick={() => setScreen('home')} className="text-white/60 hover:text-white text-sm transition">← {t.back}</button></div></div>
      </div>
    );
  }
  if (screen === 'register') { return ( <div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black flex items-center justify-center p-6"><LangButton/><div className="w-full max-w-2xl"><div className="bg-slate-900/90 backdrop-blur-xl rounded-2xl p-8 border border-white/10 shadow-2xl"><div className="mb-6"><div className="inline-flex items-center gap-2 bg-green-500/20 backdrop-blur-sm px-3 py-1.5 rounded-full mb-4"><span className="w-2 h-2 bg-green-400 rounded-full"></span><span className="text-green-300 text-xs font-medium">STUDENT RIDE-SHARING PLATFORM</span></div><h2 className="text-3xl font-bold text-white mb-2">{t.createOne}</h2><p className="text-white/60 mb-4">Join the verified student network</p></div><div className="flex gap-3 mb-6 flex-wrap"><div className="flex items-center gap-2 bg-slate-800/50 px-3 py-2 rounded-lg border border-white/10"><span className="text-lg">🎓</span><span className="text-white/70 text-xs">Verified students</span></div><div className="flex items-center gap-2 bg-slate-800/50 px-3 py-2 rounded-lg border border-white/10"><span className="text-lg">🔒</span><span className="text-white/70 text-xs">Secure access</span></div></div><div className="grid grid-cols-2 gap-4 mb-4"><div><label className="text-white/80 text-sm block mb-2">{t.name}</label><input type="text" placeholder="Your Full Name" className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2.5 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div><div><label className="text-white/80 text-sm block mb-2">Student ID</label><input type="text" placeholder="44xxxxxx" className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2.5 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div></div><div className="mb-4"><label className="text-white/80 text-sm block mb-2">{t.studentEmail}</label><input type="email" placeholder="student@imamu.edu.sa" className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2.5 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div><div className="grid grid-cols-2 gap-4 mb-6"><div><label className="text-white/80 text-sm block mb-2">{t.password}</label><input type="password" className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2.5 text-white focus:outline-none focus:border-blue-400" /></div><div><label className="text-white/80 text-sm block mb-2">Confirm</label><input type="password" className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-2.5 text-white focus:outline-none focus:border-blue-400" /></div></div><button className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg transition shadow-lg">{t.register}</button><p className="text-center text-white/60 text-sm mt-6">Already have an account?{' '}<button onClick={() => setScreen('login')} className="text-blue-400 hover:text-blue-300 transition">{t.login}</button></p></div><div className="text-center mt-6"><button onClick={() => setScreen('home')} className="text-white/60 hover:text-white text-sm transition">← {t.back}</button></div></div></div>); }
  if (screen === 'forgot') { return ( <div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black flex items-center justify-center p-6"><LangButton/><div className="w-full max-w-md"><div className="bg-slate-900/90 backdrop-blur-xl rounded-2xl p-8 border border-white/10 shadow-2xl"><div className="mb-6"><div className="inline-flex items-center gap-2 bg-green-500/20 backdrop-blur-sm px-3 py-1.5 rounded-full mb-4"><span className="w-2 h-2 bg-green-400 rounded-full"></span><span className="text-green-300 text-xs font-medium">STUDENT RIDE-SHARING</span></div><h2 className="text-3xl font-bold text-white mb-2">Forgot your password?</h2><p className="text-white/60">Enter your email for a reset link.</p></div><div className="space-y-4"><div><label className="text-white/80 text-sm block mb-2">{t.studentEmail}</label><input type="email" placeholder="student@imamu.edu.sa" className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div><button className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg transition shadow-lg">Send reset link</button></div><div className="flex items-center justify-between mt-8 pt-6 border-t border-white/10"><button onClick={() => setScreen('login')} className="text-blue-400 hover:text-blue-300 text-sm">{t.back}</button><button onClick={() => setScreen('register')} className="text-blue-400 hover:text-blue-300 text-sm">{t.createOne}</button></div></div></div></div>); }

  if (screen === 'driver') {
    const pendingRequests = globalRideRequests.filter(r => r.status === 'pending');
    const acceptedRequests = globalRideRequests.filter(r => r.status === 'accepted' || (r.status === 'completed' && !r.completed));
    const allReviews = globalRideRequests.flatMap(r => r.reviews || []);
    const averageRating = allReviews.length > 0 ? (allReviews.reduce((sum, r) => sum + r.stars, 0) / allReviews.length).toFixed(1) : '0.0';
    
    const acceptRequest = (requestId) => {
      const request = globalRideRequests.find(r => r.id === requestId);
      if (request) { request.status = 'accepted'; request.tripStatus = 'going_to_pickup'; request.driverInfo = { name: 'Khaled Alotaibi', rating: averageRating, rides: '45' }; showNotif('✅ Request accepted', 'success'); setRefreshKey(prev => prev + 1); }
    };
    const rejectRequest = (requestId) => {
      const request = globalRideRequests.find(r => r.id === requestId);
      if (request) { request.status = 'rejected'; showNotif('❌ Request rejected', 'error'); setRefreshKey(prev => prev + 1); }
    };
    const updateTripStatus = (requestId, newStatus) => {
      const request = globalRideRequests.find(r => r.id === requestId);
      if (request) {
        request.tripStatus = newStatus;
        if (newStatus === 'completed') {
            request.completed = true; 
            request.status = 'completed'; 
        }
        const statusMessages = { 'going_to_pickup': '🚗 Going to pickup location', 'arrived_pickup': '📍 Arrived at pickup', 'trip_started': '🚙 Trip started', 'arrived_destination': '🎉 Arrived at destination', 'completed': '✅ Trip completed' };
        showNotif(statusMessages[newStatus], 'success');
        setRefreshKey(prev => prev + 1);
      }
    };
    const showPassengerLocation = (request) => {
      if (currentLocation && request.from) { const geocoder = new google.maps.Geocoder(); geocoder.geocode({ address: request.from }, (results, status) => { if (status === 'OK') { pendingRouteRef.current = results[0].geometry.location; setShowMap(true); } }); } else { setShowMap(true); }
    };

    return (
      <div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black pb-12">
        <LangButton/>
        {showNotification && (<div className={`fixed top-6 right-6 px-6 py-3 rounded-lg shadow-lg z-50 ${notificationType === 'success' ? 'bg-green-500' : 'bg-red-500'} text-white font-medium`}>{notificationMessage}</div>)}
        {showReviewsModal && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-3xl bg-slate-900 rounded-2xl shadow-2xl max-h-[80vh] overflow-hidden"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">⭐ {t.reviews} ({allReviews.length})</h3><button onClick={() => setShowReviewsModal(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div className="p-6 overflow-y-auto max-h-[calc(80vh-80px)]">{allReviews.length > 0 ? (<div className="space-y-4">{allReviews.map((review) => (<div key={review.id} className="bg-slate-800/50 rounded-lg p-4 border border-white/10"><div className="flex justify-between items-start mb-2"><div><p className="text-white font-semibold">{review.passengerName}</p><p className="text-white/60 text-xs">{review.date}</p></div><div className="flex gap-1">{[...Array(5)].map((_, i) => (<span key={i} className={`text-lg ${i < review.stars ? 'text-yellow-400' : 'text-gray-600'}`}>⭐</span>))}</div></div><p className="text-white/80 text-sm">{review.comment || 'No comment provided'}</p></div>))}</div>) : (<div className="text-center py-12"><p className="text-6xl mb-4">⭐</p><p className="text-white/60">No reviews yet</p></div>)}</div></div></div>)}
        {showChat && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-2xl bg-slate-900 rounded-2xl shadow-2xl flex flex-col max-h-[80vh]"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">💬 {t.chat} {currentChatWith}</h3><button onClick={() => setShowChat(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div className="flex-1 overflow-y-auto p-6 space-y-4">{chatMessages.map((msg) => (<div key={msg.id} className={`flex ${msg.sender === 'driver' ? 'justify-end' : 'justify-start'}`}><div className={`max-w-xs px-4 py-3 rounded-2xl ${msg.sender === 'driver' ? 'bg-green-500 text-white' : 'bg-slate-800 text-white'}`}><p className="text-sm">{msg.text}</p><p className="text-xs opacity-70 mt-1">{msg.time}</p></div></div>))}</div><div className="p-6 border-t border-white/10 flex gap-3"><input type="text" placeholder="Type a message..." value={newMessage} onChange={(e) => setNewMessage(e.target.value)} onKeyPress={(e) => e.key === 'Enter' && sendMessage()} className="flex-1 bg-slate-800 border border-white/10 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /><button onClick={sendMessage} className="bg-green-500 hover:bg-green-600 px-6 py-3 rounded-lg text-white font-semibold">📤</button></div></div></div>)}
        {showMap && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-4xl bg-slate-900 rounded-2xl shadow-2xl overflow-hidden"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">🗺️ {t.viewMap}</h3><button onClick={() => setShowMap(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div ref={mapRef} className="w-full h-[500px]"></div></div></div>)}
        <div className="container mx-auto px-6 py-8"><div className="flex items-center justify-between mb-8"><div><div className="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm px-3 py-1.5 rounded-full mb-3"><span className="w-2 h-2 bg-green-400 rounded-full"></span><span className="text-white text-xs font-medium">{t.driverDashboard}</span></div><h1 className="text-4xl font-bold text-white">🚙 {t.driverPanel}</h1></div><div className="flex gap-3"><button onClick={() => setScreen('profile')} className="bg-purple-500 hover:bg-purple-600 text-white px-6 py-2.5 rounded-lg font-semibold">👤 {t.profile}</button><button onClick={() => setScreen('history')} className="bg-orange-500 hover:bg-orange-600 text-white px-6 py-2.5 rounded-lg font-semibold">📜 {t.history}</button><button onClick={() => setShowReviewsModal(true)} className="bg-yellow-500 hover:bg-yellow-600 text-white px-6 py-2.5 rounded-lg font-semibold">⭐ {t.reviews}</button><button onClick={() => setShowMap(true)} className="bg-blue-500 hover:bg-blue-600 text-white px-6 py-2.5 rounded-lg">🗺️ {t.viewMap}</button><button onClick={handleLogout} className="bg-slate-800/50 hover:bg-slate-800 text-white px-6 py-2.5 rounded-lg border border-white/10">{t.logout}</button></div></div><div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 mb-6 border border-white/10"><h2 className="text-2xl font-bold text-white mb-2">Welcome! 🎉</h2><p className="text-white/70">You have {pendingRequests.length} {t.newRequests}</p></div>
          {pendingRequests.length > 0 ? (
            <div className="mb-8"><h3 className="text-2xl font-bold text-white mb-4">🔔 {t.newRequests}</h3><div className="space-y-4">{pendingRequests.map((request) => (<div key={request.id} className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10"><div className="flex justify-between items-start mb-4"><div><h4 className="text-xl font-bold text-white">👤 {request.passengerName}</h4><p className="text-yellow-400">⭐ {request.passengerRating}</p></div><div className="text-right"><p className="text-2xl font-bold text-green-400">{request.price} {t.sar}</p><p className="text-white/60 text-sm">{request.time}</p></div></div><div className="bg-slate-800/50 rounded-lg p-4 mb-4"><p className="text-white mb-2">📍 {t.from}: {request.from}</p><p className="text-white mb-2">🎯 {t.to}: {request.to}</p><div className="flex gap-4 mt-3 pt-3 border-t border-white/10"><p className="text-white/80 text-sm">👥 {t.passengers}: <span className="text-green-400 font-semibold">{request.passengerCount}</span></p><p className="text-white/80 text-sm">💳 {t.payment}: <span className="text-blue-400 font-semibold">{request.paymentMethod === 'cash' ? t.cash : request.paymentMethod === 'card' ? t.creditCard : t.wallet}</span></p></div></div><div className="flex gap-3"><button onClick={() => acceptRequest(request.id)} className="flex-1 bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg">✅ {t.accept}</button><button onClick={() => rejectRequest(request.id)} className="flex-1 bg-red-500 hover:bg-red-600 text-white font-semibold py-3 rounded-lg">❌ {t.reject}</button></div></div>))}</div></div>
          ) : (<div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-12 border border-white/10 text-center mb-8"><p className="text-6xl mb-4">📭</p><p className="text-white/60">{t.noRequests}</p></div>)}
          {acceptedRequests.length > 0 && (
            <div className="mb-8"><h3 className="text-2xl font-bold text-white mb-4">✅ {t.activeTrips}</h3><div className="space-y-4">{acceptedRequests.map((request) => {if (request.tripStatus === 'completed') return null; const tripStatus = request.tripStatus || 'going_to_pickup'; const statusConfig = { 'going_to_pickup': { label: '🚗 Going to Pickup', color: 'blue', next: 'arrived_pickup', nextLabel: '📍 Arrived at Pickup' }, 'arrived_pickup': { label: '📍 At Pickup Location', color: 'yellow', next: 'trip_started', nextLabel: '🚙 Start Trip' }, 'trip_started': { label: '🚙 Trip in Progress', color: 'purple', next: 'arrived_destination', nextLabel: '🎯 Arrived at Destination' }, 'arrived_destination': { label: '🎯 At Destination', color: 'green', next: 'completed', nextLabel: '✅ Complete Trip' } }; const currentStatus = statusConfig[tripStatus]; return (<div key={request.id} className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10"><div className="flex justify-between items-start mb-4"><div><h4 className="text-xl font-bold text-white">👤 {request.passengerName}</h4><div className={`inline-block px-3 py-1 rounded-full text-sm font-medium mt-2 ${currentStatus.color === 'blue' ? 'bg-blue-500/20 text-blue-400' : currentStatus.color === 'yellow' ? 'bg-yellow-500/20 text-yellow-400' : currentStatus.color === 'purple' ? 'bg-purple-500/20 text-purple-400' : 'bg-green-500/20 text-green-400'}`}>{currentStatus.label}</div></div><div className="text-right"><p className="text-2xl font-bold text-green-400">{request.price} {t.sar}</p><p className="text-white/60 text-sm">{request.time}</p></div></div><div className="bg-slate-800/50 rounded-lg p-4 mb-4"><p className="text-white mb-2">📍 {t.from}: {request.from}</p><p className="text-white mb-2">🎯 {t.to}: {request.to}</p><div className="flex gap-4 mt-3 pt-3 border-t border-white/10"><p className="text-white/80 text-sm">👥 {t.passengers}: <span className="text-green-400 font-semibold">{request.passengerCount}</span></p><p className="text-white/80 text-sm">💳 {t.payment}: <span className="text-blue-400 font-semibold">{request.paymentMethod === 'cash' ? t.cash : request.paymentMethod === 'card' ? t.creditCard : t.wallet}</span></p></div></div><div className="bg-blue-500/10 border border-blue-500/30 rounded-lg p-4 mb-4"><p className="text-white font-semibold mb-3">📱 {t.passengerContact}</p><div className="flex items-center justify-between"><div><p className="text-white text-sm">📧 {request.passenger}</p><p className="text-yellow-400 text-sm">⭐ {request.passengerRating}</p></div></div></div><div className="grid grid-cols-2 gap-3 mb-3"><button onClick={() => openChat(request.passengerName)} className="bg-blue-500 hover:bg-blue-600 text-white px-4 py-3 rounded-lg font-semibold">💬 {t.chat}</button><button onClick={() => showPassengerLocation(request)} className="bg-purple-500 hover:bg-purple-600 text-white px-4 py-3 rounded-lg font-semibold">📍 {t.viewLocation}</button></div>{currentStatus.next && (<button onClick={() => updateTripStatus(request.id, currentStatus.next)} className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg">{currentStatus.nextLabel}</button>)}</div>); })}</div></div>
          )}
          <div className="grid grid-cols-2 md:grid-cols-4 gap-4"><div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10 text-center"><p className="text-4xl mb-2">🚗</p><p className="text-3xl font-bold text-white">12</p><p className="text-white/60">{t.trips}</p></div><div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10 text-center"><p className="text-4xl mb-2">👥</p><p className="text-3xl font-bold text-white">45</p><p className="text-white/60">{t.passengers}</p></div><div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10 text-center"><p className="text-4xl mb-2">⭐</p><p className="text-3xl font-bold text-white">{averageRating}</p><p className="text-white/60">{t.rating}</p></div><div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10 text-center"><p className="text-4xl mb-2">💰</p><p className="text-3xl font-bold text-white">350</p><p className="text-white/60">{t.sar}</p></div></div>
        </div>
      </div>
    );
  }

  const myRequests = globalRideRequests.filter(r => r.passenger === email && !r.rating); // Show active until rated
  const myScheduledRides = scheduledRides.filter(r => r.passenger === email);
  const walletBalance = userProfiles[email]?.walletBalance || 0;
  const transactions = userProfiles[email]?.transactions || [];
  const myInstallments = userProfiles[email]?.installments || [];

  return (
    <div className="min-h-screen bg-gradient-to-br from-green-400 via-blue-600 to-black pb-12">
      <LangButton/>
      {showNotification && (<div className={`fixed top-6 right-6 px-6 py-3 rounded-lg shadow-lg z-50 ${notificationType === 'success' ? 'bg-green-500' : 'bg-red-500'} text-white font-medium`}>{notificationMessage}</div>)}
      
      {showWalletModal && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-md bg-slate-900 rounded-2xl shadow-2xl"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">💰 {t.myWallet}</h3><button onClick={() => setShowWalletModal(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div className="p-6"><div className="bg-gradient-to-br from-green-500 to-blue-600 rounded-2xl p-6 mb-6 text-center"><p className="text-white/80 text-sm mb-2">{t.currentBalance}</p><p className="text-5xl font-bold text-white mb-1">{walletBalance.toFixed(2)}</p><p className="text-white/80 text-sm">{t.sar}</p></div><div className="mb-4"><label className="text-white/80 text-sm block mb-2">{t.depositAmount} ({t.sar})</label><input type="number" placeholder="Enter amount" value={depositAmount} onChange={(e) => setDepositAmount(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div><button onClick={handleDeposit} className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg mb-3">💳 {t.addMoney}</button><button onClick={() => setShowTransactionsModal(true)} className="w-full bg-blue-500 hover:bg-blue-600 text-white font-semibold py-3 rounded-lg mb-4">📊 {t.viewTransactions}</button><div className="border-t border-white/10 pt-4"><h4 className="text-white font-bold mb-3">Split Payments</h4><button onClick={() => setShowInstallmentsListModal(true)} className="w-full bg-slate-800 hover:bg-slate-700 text-white font-semibold py-3 rounded-lg border border-white/10">📋 View Active Splits</button></div></div></div></div>)}
      {showTransactionsModal && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-2xl bg-slate-900 rounded-2xl shadow-2xl max-h-[80vh] overflow-hidden"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">📊 {t.transactionHistory}</h3><button onClick={() => setShowTransactionsModal(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div className="p-6 overflow-y-auto max-h-[calc(80vh-80px)]">{transactions.length > 0 ? (<div className="space-y-3">{transactions.map((transaction) => (<div key={transaction.id} className="bg-slate-800/50 rounded-lg p-4 border border-white/10 flex items-center justify-between"><div className="flex items-center gap-4"><div className={`text-3xl ${transaction.type === 'deposit' ? 'text-green-400' : 'text-red-400'}`}>{transaction.type === 'deposit' ? '💰' : '💸'}</div><div><p className="text-white font-semibold">{transaction.description}</p><p className="text-white/60 text-xs">{transaction.date}</p></div></div><div className={`text-xl font-bold ${transaction.amount > 0 ? 'text-green-400' : 'text-red-400'}`}>{transaction.amount > 0 ? '+' : ''}{transaction.amount} {t.sar}</div></div>))}</div>) : (<div className="text-center py-12"><p className="text-6xl mb-4">📭</p><p className="text-white/60">No transactions yet</p></div>)}</div></div></div>)}
      {showInstallmentModal && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-md bg-slate-900 rounded-2xl shadow-2xl"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">💳 Choose Split Plan</h3><button onClick={() => setShowInstallmentModal(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div className="p-6 space-y-4"><div><label className="text-white/80 text-sm block mb-2">Trip Price: {currentInstallmentPrice || 'Calculating...'} {t.sar}</label></div><div><label className="text-white/80 text-sm block mb-2">Number of Splits</label><select value={installmentCount} onChange={(e) => setInstallmentCount(Number(e.target.value))} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-blue-400"><option value={2}>2 Splits ({(currentInstallmentPrice / 2).toFixed(2)} {t.sar} each)</option><option value={3}>3 Splits ({(currentInstallmentPrice / 3).toFixed(2)} {t.sar} each)</option><option value={4}>4 Splits ({(currentInstallmentPrice / 4).toFixed(2)} {t.sar} each)</option><option value={5}>5 Splits ({(currentInstallmentPrice / 5).toFixed(2)} {t.sar} each)</option></select></div><div className="bg-blue-500/10 border border-blue-500/30 rounded-lg p-4"><p className="text-blue-300 text-sm">💡 First payment will be deducted now. Remaining payments will be auto-deducted periodically.</p></div><button onClick={handleInstallmentPayment} className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg">Confirm & Pay First Split</button></div></div></div>)}
      {showInstallmentsListModal && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-2xl bg-slate-900 rounded-2xl shadow-2xl max-h-[80vh] overflow-hidden"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">📋 My Splits</h3><button onClick={() => setShowInstallmentsListModal(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div className="p-6 overflow-y-auto max-h-[calc(80vh-80px)]">{myInstallments.length > 0 ? (<div className="space-y-3">{myInstallments.map((inst) => (<div key={inst.id} className="bg-slate-800/50 rounded-lg p-4 border border-white/10"><div className="flex justify-between items-center mb-2"><div><p className="text-white font-semibold">Split {inst.installmentNumber} of {inst.totalInstallments}</p><p className="text-white/60 text-xs">{inst.tripDescription}</p></div><div className="text-right"><p className="text-xl font-bold text-white">{inst.amount} {t.sar}</p><span className={`text-xs px-2 py-1 rounded ${inst.status === 'paid' ? 'bg-green-500/20 text-green-400' : 'bg-yellow-500/20 text-yellow-400'}`}>{inst.status === 'paid' ? '✅ PAID' : '⏳ PENDING'}</span></div></div><div className="flex justify-between text-xs text-white/40"><span>Due: {new Date(inst.dueDate).toLocaleString()}</span>{inst.status === 'paid' && <span>Paid on: {new Date(inst.paidDate).toLocaleDateString()}</span>}</div></div>))}</div>) : (<div className="text-center py-12"><p className="text-6xl mb-4">💳</p><p className="text-white/60">No active splits</p></div>)}</div></div></div>)}
      {showEmergencyModal && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-md bg-slate-900 rounded-2xl shadow-2xl border-2 border-red-500"><div className="flex items-center justify-between p-6 border-b border-white/10 bg-red-500/20"><h3 className="text-xl font-bold text-white">🚨 Emergency Alert</h3><button onClick={() => setShowEmergencyModal(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div className="p-6 space-y-4"><div className="bg-red-500/10 border border-red-500/30 rounded-lg p-4"><p className="text-red-400 font-semibold mb-2">This will send immediately:</p><div className="space-y-1 text-sm text-white/80"><p>• Your current GPS location</p><p>• Driver information</p><p>• Trip details</p><p>• Alert to university security</p></div></div><div><label className="text-white/80 text-sm block mb-2">Describe the emergency:</label><textarea value={emergencyDescription} onChange={(e) => setEmergencyDescription(e.target.value)} placeholder="What's happening? Be as specific as possible..." rows="4" className="w-full bg-slate-800/50 border border-red-500/30 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-red-400 resize-none"></textarea></div><button onClick={handleEmergencyAlert} className="w-full bg-red-500 hover:bg-red-600 text-white font-bold py-4 rounded-lg emergency-pulse shadow-lg">🚨 SEND EMERGENCY ALERT</button><p className="text-xs text-white/40 text-center">Response time: Under 60 seconds</p></div></div></div>)}
      {showScheduleModal && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-md bg-slate-900 rounded-2xl shadow-2xl"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">📅 {t.scheduleRide}</h3><button onClick={() => setShowScheduleModal(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div className="p-6 space-y-4"><div><label className="text-white/80 text-sm block mb-2">📅 {t.date}</label><input type="date" value={scheduleDate} onChange={(e) => setScheduleDate(e.target.value)} min={new Date().toISOString().split('T')[0]} className={`w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-blue-400 ${scheduleDate ? 'has-value' : ''}`} /></div><div><label className="text-white/80 text-sm block mb-2">⏰ {t.time}</label><input type="time" value={scheduleTime} onChange={(e) => setScheduleTime(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-blue-400" /></div><div><label className="text-white/80 text-sm block mb-2">🔁 {t.repeat}</label><select value={scheduleRecurring} onChange={(e) => setScheduleRecurring(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-blue-400"><option value="once">{t.once}</option><option value="daily">{t.daily}</option><option value="weekly">{t.weekly}</option><option value="weekdays">{t.weekdays}</option></select></div><div className="bg-blue-500/10 border border-blue-500/30 rounded-lg p-4"><p className="text-blue-300 text-sm">📍 {t.from}: {pickupLocation || 'Not set'}<br/>🎯 {t.to}: {destination || 'Not set'}</p></div><button onClick={handleScheduleRide} className="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg">📅 {t.scheduleRide}</button></div></div></div>)}

      {showChat && (
        <div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6">
          <div className="w-full max-w-2xl bg-slate-900 rounded-2xl shadow-2xl flex flex-col max-h-[80vh]">
            <div className="flex items-center justify-between p-6 border-b border-white/10">
              <h3 className="text-xl font-bold text-white">💬 {t.chat} {currentChatWith}</h3>
              <button onClick={() => setShowChat(false)} className="text-white/60 hover:text-white text-2xl">✕</button>
            </div>
            <div className="flex-1 overflow-y-auto p-6 space-y-4">
              {chatMessages.map((msg) => (
                <div key={msg.id} className={`flex ${msg.sender === 'passenger' ? 'justify-end' : 'justify-start'}`}>
                  <div className={`max-w-xs px-4 py-3 rounded-2xl ${msg.sender === 'passenger' ? 'bg-green-500 text-white' : 'bg-slate-800 text-white'}`}>
                    <p className="text-sm">{msg.text}</p>
                    <p className="text-xs opacity-70 mt-1">{msg.time}</p>
                  </div>
                </div>
              ))}
            </div>
            <div className="p-6 border-t border-white/10 flex gap-3">
              <input type="text" placeholder="Type a message..." value={newMessage} onChange={(e) => setNewMessage(e.target.value)} onKeyPress={(e) => e.key === 'Enter' && sendMessage()} className="flex-1 bg-slate-800 border border-white/10 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" />
              <button onClick={sendMessage} className="bg-green-500 hover:bg-green-600 px-6 py-3 rounded-lg text-white font-semibold">📤</button>
            </div>
          </div>
        </div>
      )}

      {showTrackingModal && trackingData && (
        <div className="fixed inset-0 bg-black/80 backdrop-blur-sm z-50 flex items-end justify-center sm:items-center p-4">
          <div className="w-full max-w-lg bg-[#0f172a] rounded-t-3xl sm:rounded-3xl border border-white/10 shadow-2xl overflow-hidden relative">
            <div className="flex items-center justify-between p-5 border-b border-white/5"><div className="flex items-center gap-2"><span className="text-red-500 text-xl">📍</span><h3 className="text-lg font-bold text-white">{t.trackLive}</h3></div><button onClick={closeTracking} className="text-white/60 hover:text-white text-xl">✕</button></div>
            <div className="p-6 flex flex-col items-center justify-center text-center">
                <div className="mb-6 relative w-full h-32 flex items-center justify-center bg-[#1e293b]/50 rounded-2xl border border-white/5"><div className="text-7xl car-float drop-shadow-2xl">🚖</div><div className="absolute bottom-4 text-xs text-white/40 font-mono tracking-widest">CONNECTING TO GPS...</div></div>
                <h2 className="text-2xl font-bold text-white mb-2">Driver is on the way</h2><p className="text-white/50 text-sm mb-8">Stay tuned for updates</p>
                <div className="grid grid-cols-3 gap-4 w-full mb-6"><div className="bg-[#1e293b] p-4 rounded-xl border border-white/5 flex flex-col items-center"><span className="text-white/40 text-xs mb-1 uppercase tracking-wider">ETA</span><span className="text-green-400 text-xl font-bold">{Math.ceil(trackingData.eta)} min</span></div><div className="bg-[#1e293b] p-4 rounded-xl border border-white/5 flex flex-col items-center"><span className="text-white/40 text-xs mb-1 uppercase tracking-wider">Speed</span><span className="text-blue-400 text-xl font-bold">{Math.round(trackingData.speed)} km/h</span></div><div className="bg-[#1e293b] p-4 rounded-xl border border-white/5 flex flex-col items-center"><span className="text-white/40 text-xs mb-1 uppercase tracking-wider">Distance</span><span className="text-yellow-400 text-xl font-bold">{trackingData.distance.toFixed(1)} km</span></div></div>
                <div className="w-full bg-blue-500/10 border border-blue-500/20 rounded-lg py-3 px-4 flex items-center justify-center gap-2"><span className="text-blue-400 text-lg animate-pulse">💡</span><span className="text-blue-200 text-xs">Location updates every 2 seconds</span></div>
                {trackingData.status === 'arrived' && (<button onClick={closeTracking} className="w-full mt-4 bg-green-500 hover:bg-green-600 text-white font-bold py-4 rounded-xl shadow-lg transition transform hover:scale-[1.02]">Driver Arrived - Complete Trip</button>)}
            </div>
          </div>
        </div>
      )}

      {/* RATING MODAL (Auto Pop-up) */}
      {showRatingModal && (
        <div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6">
          <div className="w-full max-w-md bg-slate-900 rounded-2xl shadow-2xl border border-yellow-500/20">
            <div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">⭐ Trip Completed</h3></div>
            <div className="p-6">
              <p className="text-white/70 text-sm mb-4 text-center">Your trip has finished. How was your experience?</p>
              <div className="flex justify-center gap-2 mb-6">{[1, 2, 3, 4, 5].map((star) => (<button key={star} onClick={() => setRatingData({...ratingData, stars: star})} className="text-4xl transition hover:scale-110">{star <= ratingData.stars ? '⭐' : '☆'}</button>))}</div>
              <div className="mb-6"><label className="text-white/80 text-sm block mb-2">Add a comment (optional)</label><textarea value={ratingData.comment} onChange={(e) => setRatingData({...ratingData, comment: e.target.value})} placeholder="Share your experience..." rows="4" className="w-full bg-slate-800/50 border border-white/10 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400 resize-none"></textarea></div>
              <button onClick={submitRating} className="w-full bg-yellow-500 hover:bg-yellow-600 text-white font-bold py-3 rounded-lg shadow-lg">Submit Rating</button>
            </div>
          </div>
        </div>
      )}

      {/* NEW: MAP MODAL */}
      {showMap && (<div className="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-6"><div className="w-full max-w-4xl bg-slate-900 rounded-2xl shadow-2xl overflow-hidden"><div className="flex items-center justify-between p-6 border-b border-white/10"><h3 className="text-xl font-bold text-white">🗺️ {t.viewMap}</h3><button onClick={() => setShowMap(false)} className="text-white/60 hover:text-white text-2xl">✕</button></div><div ref={mapRef} className="w-full h-[500px]"></div></div></div>)}

      {/* DASHBOARD */}
      <div className="container mx-auto px-6 py-8">
        <div className="flex items-center justify-between mb-8">
          <div><div className="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm px-3 py-1.5 rounded-full mb-3"><span className="w-2 h-2 bg-green-400 rounded-full"></span><span className="text-white text-xs font-medium">{t.passengerDashboard}</span></div><h1 className="text-4xl font-bold text-white">🎒 {t.passengerPanel}</h1></div>
          <div className="flex gap-3"><button onClick={() => setShowWalletModal(true)} className="bg-green-500 hover:bg-green-600 text-white px-6 py-2.5 rounded-lg font-semibold">💰 {t.wallet}: {walletBalance.toFixed(0)} {t.sar}</button><button onClick={() => setScreen('profile')} className="bg-purple-500 hover:bg-purple-600 text-white px-6 py-2.5 rounded-lg font-semibold">👤 {t.profile}</button><button onClick={() => setScreen('history')} className="bg-orange-500 hover:bg-orange-600 text-white px-6 py-2.5 rounded-lg font-semibold">📜 {t.history}</button><button onClick={() => setShowMap(true)} className="bg-blue-500 hover:bg-blue-600 text-white px-6 py-2.5 rounded-lg">🗺️ {t.viewMap}</button><button onClick={handleLogout} className="bg-slate-800/50 hover:bg-slate-800 text-white px-6 py-2.5 rounded-lg border border-white/10">{t.logout}</button></div>
        </div>
        <div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-8 mb-6 border border-white/10">
          <h2 className="text-2xl font-bold text-white mb-6">📍 {t.requestNewRide}</h2>
          <div className="space-y-4">
            <div><label className="text-white/80 text-sm block mb-2">{t.pickupLocation} {currentLocation && <span className="text-green-400 text-xs">📍 GPS Enabled</span>}</label><input type="text" placeholder="Example: University - Gate 2" value={pickupLocation} onChange={(e) => setPickupLocation(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div>
            <div><label className="text-white/80 text-sm block mb-2">{t.destination}</label><input type="text" placeholder="Example: Al Nargis District" value={destination} onChange={(e) => setDestination(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white placeholder-white/40 focus:outline-none focus:border-blue-400" /></div>
            <div className="grid grid-cols-2 gap-4">
              <div><label className="text-white/80 text-sm block mb-2">👥 {t.numberOfPassengers}</label><select value={passengerCount} onChange={(e) => setPassengerCount(Number(e.target.value))} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-blue-400"><option value={1}>1 {t.passenger}</option><option value={2}>2 {t.passengers}</option><option value={3}>3 {t.passengers}</option><option value={4}>4 {t.passengers}</option></select></div>
              <div>
                <label className="text-white/80 text-sm block mb-2">💳 {t.paymentMethod}</label>
                <select value={paymentMethod} onChange={(e) => setPaymentMethod(e.target.value)} className="w-full bg-slate-800/50 border border-blue-500/30 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-blue-400">
                    <option value="cash">💵 {t.cash}</option>
                    <option value="card">💳 {t.creditCard}</option>
                    <option value="wallet">💰 {t.wallet} ({walletBalance.toFixed(0)} {t.sar})</option>
                    <option value="installment">📉 Split (Pay later)</option>
                </select>
              </div>
            </div>
            <div className="grid grid-cols-2 gap-3">
              <button onClick={requestRide} className="bg-green-500 hover:bg-green-600 text-white font-semibold py-3 rounded-lg transition shadow-lg">🚀 {t.requestNow}</button>
              <button onClick={() => { if (!pickupLocation || !destination) { showNotif('⚠️ Enter location and destination first', 'error'); return; } setShowScheduleModal(true); }} className="bg-blue-500 hover:bg-blue-600 text-white font-semibold py-3 rounded-lg transition shadow-lg">📅 {t.schedule}</button>
            </div>
          </div>
        </div>

        {myScheduledRides.length > 0 && (
          <div className="mb-8">
            <h3 className="text-2xl font-bold text-white mb-4">📅 {t.scheduledRides}</h3>
            <div className="space-y-4">
              {myScheduledRides.map((ride) => (
                <div key={ride.id} className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10">
                  <div className="flex justify-between items-start mb-4"><div><div className="inline-block px-3 py-1 rounded-full text-sm font-medium mb-2 bg-blue-500/20 text-blue-400">📅 {t.scheduled}</div><p className="text-white/60 text-sm">{ride.scheduleDate} at {ride.scheduleTime}{ride.recurring !== 'once' && ` - ${ride.recurring}`}</p></div><div className="text-right"><p className="text-2xl font-bold text-green-400">{ride.price} {t.sar}</p></div></div>
                  <div className="bg-slate-800/50 rounded-lg p-4 mb-4"><p className="text-white mb-2">📍 {t.from}: {ride.from}</p><p className="text-white mb-2">🎯 {t.to}: {ride.to}</p><div className="flex gap-4 mt-3 pt-3 border-t border-white/10"><p className="text-white/80 text-sm">👥 {t.passengers}: <span className="text-green-400 font-semibold">{ride.passengerCount}</span></p><p className="text-white/80 text-sm">💳 {t.payment}: <span className="text-blue-400 font-semibold">{ride.paymentMethod === 'cash' ? t.cash : ride.paymentMethod === 'card' ? t.creditCard : ride.paymentMethod === 'installment' ? 'Split' : t.wallet}</span></p></div></div>
                  <button onClick={() => { scheduledRides = scheduledRides.filter(r => r.id !== ride.id); showNotif('✅ Scheduled ride cancelled', 'success'); setRefreshKey(prev => prev + 1); }} className="w-full bg-red-500 hover:bg-red-600 text-white font-semibold py-2 rounded-lg">❌ {t.cancelSchedule}</button>
                </div>
              ))}
            </div>
          </div>
        )}

        <div className="mb-8">
          <h3 className="text-2xl font-bold text-white mb-4">📋 {t.myRequests}</h3>
          {myRequests.length > 0 ? (
            <div className="space-y-4">
              {myRequests.map((request) => (
                <div key={request.id} className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10">
                  <div className="flex justify-between items-start mb-4">
                    <div><div className={`inline-block px-3 py-1 rounded-full text-sm font-medium mb-2 ${request.status === 'pending' ? 'bg-yellow-500/20 text-yellow-400' : request.status === 'accepted' ? 'bg-green-500/20 text-green-400' : 'bg-red-500/20 text-red-400'}`}>{request.status === 'pending' ? `⏳ ${t.pending}` : request.status === 'accepted' ? `✅ ${t.accepted}` : `❌ ${t.rejected}`}</div><p className="text-white/60 text-sm">{request.date} - {request.time}</p></div>
                    <div className="text-right"><p className="text-2xl font-bold text-green-400">{request.price} {t.sar}</p></div>
                  </div>
                  <div className="bg-slate-800/50 rounded-lg p-4 mb-4"><p className="text-white mb-2">📍 {t.from}: {request.from}</p><p className="text-white mb-2">🎯 {t.to}: {request.to}</p><div className="flex gap-4 mt-3 pt-3 border-t border-white/10"><p className="text-white/80 text-sm">👥 {t.passengers}: <span className="text-green-400 font-semibold">{request.passengerCount}</span></p><p className="text-white/80 text-sm">💳 {t.payment}: <span className="text-blue-400 font-semibold">{request.paymentMethod === 'cash' ? t.cash : request.paymentMethod === 'card' ? t.creditCard : request.paymentMethod === 'installment' ? 'Split' : t.wallet}</span></p></div></div>
                  {request.status === 'accepted' && request.driverInfo && (
                    <div className="bg-green-500/10 border border-green-500/30 rounded-lg p-4">
                      {/* IF COMPLETED: Show minimalist view, rating modal will pop up. */}
                      {(request.completed || request.tripStatus === 'completed') ? (
                        <div className="text-center py-4">
                            <p className="text-green-400 font-bold mb-2">✅ Trip Finished</p>
                            <p className="text-white/60 text-sm">Please rate your trip in the popup window.</p>
                        </div>
                      ) : (
                        <>
                            <p className="text-white font-semibold mb-3">🚗 {t.driverInfo}</p>
                            <div className="flex items-center justify-between mb-3"><div><p className="text-white">👤 {request.driverInfo.name}</p><p className="text-yellow-400 text-sm">⭐ {request.driverInfo.rating} ({request.driverInfo.rides} {t.trips})</p></div></div>
                            {request.emergencyReported && (<div className="bg-red-500/20 border border-red-500 rounded-lg p-3 text-center mb-3"><p className="text-red-400 font-semibold">🚨 Emergency Alert Sent</p><p className="text-white/60 text-sm">Help is on the way</p></div>)}
                            <div className="flex gap-2">
                                <button onClick={() => openChat(request.driverInfo.name)} className="flex-1 bg-blue-500 hover:bg-blue-600 text-white px-4 py-2 rounded-lg text-sm font-semibold">💬 {t.chat}</button>
                                <button onClick={() => startLiveTracking(request)} className="flex-1 bg-purple-500 hover:bg-purple-600 text-white px-4 py-2 rounded-lg text-sm font-semibold">📍 {t.trackLive}</button>
                            </div>
                            {!request.emergencyReported && (<button onClick={() => { setCurrentEmergencyRequest(request); setShowEmergencyModal(true); }} className="w-full mt-3 bg-red-500/80 hover:bg-red-600 text-white font-semibold py-2 rounded-lg text-sm emergency-pulse">🚨 Emergency - Help</button>)}
                        </>
                      )}
                    </div>
                  )}
                </div>
              ))}
            </div>
          ) : (
            <div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-12 border border-white/10 text-center"><p className="text-6xl mb-4">📭</p><p className="text-white/60">{t.noRequests}</p></div>
          )}
        </div>
        <div className="grid grid-cols-3 gap-4">
          <div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10 text-center"><p className="text-4xl mb-2">🚗</p><p className="text-3xl font-bold text-white">8</p><p className="text-white/60">{t.trips}</p></div>
          <div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10 text-center"><p className="text-4xl mb-2">💰</p><p className="text-3xl font-bold text-white">240</p><p className="text-white/60">{t.saved}</p></div>
          <div className="bg-slate-900/80 backdrop-blur-xl rounded-2xl p-6 border border-white/10 text-center"><p className="text-4xl mb-2">⭐</p><p className="text-3xl font-bold text-white">4.9</p><p className="text-white/60">{t.rating}</p></div>
        </div>
      </div>
    </div>
  );
}

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<App />);
    </script>
</body>
</html>