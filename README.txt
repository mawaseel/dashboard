MAWASEEL DASHBOARD - FULL PARTNER APP
Domain: https://dashboard.mawaseel.ps

Pages:
- index.html: Overview
- orders.html: Live partner orders with search/filter
- order.html?id=: Order details + status timeline
- earnings.html: Live commission calculations + 6-month chart
- activity.html: Timeline from order status history
- notifications.html: Latest order updates
- settings.html: Dashboard settings/account shortcuts
- login.html: Dashboard-domain login

This site reads orders from Firestore where partnerId == current user uid. It never creates or edits orders. Admin controls orders from admin.mawaseel.ps.

IMPORTANT: A static Firebase browser session is origin-specific. Because dashboard.mawaseel.ps is a separate domain, users sign in to this dashboard domain once. Their session is then remembered locally on that domain. Seamless cross-subdomain SSO requires a backend/session-cookie implementation.
