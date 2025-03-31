// GetAudit Authentication with CAPTCHA
document.addEventListener('DOMContentLoaded', function() {
    const authSystem = {
        MAX_ATTEMPTS: 5,
        LOCKOUT_TIME: 15 * 60 * 1000, // 15 minutes
        
        init() {
            this.setupEventListeners();
            this.loadAttempts();
        },
        
        setupEventListeners() {
            // Tab switching
            document.querySelectorAll('.auth-tab').forEach(tab => {
                tab.addEventListener('click', () => this.switchTab(tab));
            });
            
            // Login form
            document.getElementById('login-form').addEventListener('submit', (e) => {
                e.preventDefault();
                this.handleLogin();
            });
            
            // Registration form
            document.getElementById('register-form').addEventListener('submit', (e) => {
                e.preventDefault();
                this.handleRegistration();
            });
        },
        
        async handleLogin() {
            if (this.isAccountLocked()) {
                this.showError('login', 'Account temporarily locked. Try again later.');
                return;
            }
            
            // ... login validation ...
            
            if (invalid) {
                this.recordFailedAttempt();
            }
        },
        
        async handleRegistration() {
            // Validate CAPTCHA first
            if (!window.getAudit?.captchaResponse) {
                this.showError('register', 'Please complete the CAPTCHA verification');
                return;
            }
            
            // ... registration logic ...
        },
        
        isAccountLocked() {
            const lock = JSON.parse(localStorage.getItem('auth_lockout') || '{}');
            return lock.time && (Date.now() - lock.time < this.LOCKOUT_TIME);
        },
        
        recordFailedAttempt() {
            const attempts = JSON.parse(localStorage.getItem('failed_attempts') || '[]');
            attempts.push(Date.now());
            
            // Clean old attempts
            const recent = attempts.filter(t => Date.now() - t < 3600000); // 1 hour
            localStorage.setItem('failed_attempts', JSON.stringify(recent));
            
            if (recent.length >= this.MAX_ATTEMPTS) {
                localStorage.setItem('auth_lockout', JSON.stringify({
                    time: Date.now()
                }));
            }
        },
        
        // ... other methods ...
    };
    
    authSystem.init();
});
