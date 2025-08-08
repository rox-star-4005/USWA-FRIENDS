<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Uswa 40th Batch - Darul Huda Islamic University</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* All existing CSS styles remain the same */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
       
        body {
            background-color: #f9fafb;
            color: #2c3e50;
            line-height: 1.6;
        }
       
        header {
            background: linear-gradient(135deg, #004d40, #00796b);
            color: white;
            padding: 1.5rem 0;
            box-shadow: 0 3px 10px rgba(0,0,0,0.2);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
       
        .header-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
       
        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
        }
       
        .logo img {
            height: 60px;
            border-radius: 50%;
            border: 2px solid #fff;
        }
       
        .logo h1 {
            font-size: 1.8rem;
            font-weight: 700;
        }
       
        .logo span {
            color: #ffd54f;
        }
       
        nav {
            display: flex;
            gap: 20px;
        }
       
        nav a {
            color: white;
            text-decoration: none;
            padding: 8px 15px;
            border-radius: 5px;
            transition: all 0.3s ease;
            font-weight: 500;
        }
       
        nav a:hover, nav a.active {
            background-color: rgba(255, 255, 255, 0.15);
        }
       
        .user-actions {
            display: flex;
            gap: 15px;
            align-items: center;
        }
       
        .btn {
            padding: 8px 20px;
            border-radius: 50px;
            font-weight: 600;
            text-decoration: none;
            cursor: pointer;
            transition: all 0.3s ease;
            display: inline-block;
        }
       
        .btn-primary {
            background-color: #ffd54f;
            color: #004d40;
        }
       
        .btn-primary:hover {
            background-color: #ffb300;
            transform: translateY(-2px);
        }
       
        .btn-outline {
            border: 2px solid white;
            color: white;
        }
       
        .btn-outline:hover {
            background-color: white;
            color: #004d40;
        }
       
        .btn-success {
            background-color: #4caf50;
            color: white;
            border: none;
            padding: 8px 20px;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
       
        .btn-danger {
            background-color: #e74c3c;
            color: white;
            border: none;
            padding: 8px 20px;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
       
        .btn-logout {
            background-color: #e74c3c;
            color: white;
            border: none;
            padding: 8px 20px;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
       
        .btn-logout:hover {
            background-color: #c0392b;
        }
       
        main {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }
       
        .section {
            display: none;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            padding: 30px;
            margin-bottom: 30px;
        }
       
        .section.active {
            display: block;
        }
       
        .section-title {
            text-align: center;
            margin-bottom: 25px;
        }
       
        .section-title h2 {
            color: #004d40;
            font-size: 2.2rem;
            margin-bottom: 10px;
        }
       
        .section-title p {
            color: #666;
            max-width: 700px;
            margin: 0 auto;
        }
       
        /* Home Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url("https://i.ibb.co/bgC4c7qX/unnamed.jpg") center/cover;
            color: white;
            padding: 80px 0;
            text-align: center;
            border-radius: 10px;
            margin-bottom: 30px;
        }
       
        .hero h2 {
            font-size: 2.8rem;
            margin-bottom: 20px;
        }
       
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
        }
       
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-top: 40px;
        }
       
        .feature-card {
            background-color: #f1fdfa;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            transition: transform 0.3s ease;
        }
       
        .feature-card:hover {
            transform: translateY(-10px);
        }
       
        .feature-icon {
            background-color: #004d40;
            color: white;
            font-size: 2.5rem;
            padding: 25px;
            text-align: center;
        }
       
        .feature-content {
            padding: 20px;
        }
       
        .feature-content h3 {
            color: #004d40;
            margin-bottom: 10px;
            font-size: 1.4rem;
        }
       
        /* Gallery Section */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
       
        .gallery-item {
            position: relative;
            border-radius: 10px;
            overflow: hidden;
            height: 250px;
            cursor: pointer;
        }
       
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
       
        .gallery-item:hover img {
            transform: scale(1.1);
        }
       
        .gallery-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.6);
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.3s ease;
        }
       
        .gallery-item:hover .gallery-overlay {
            opacity: 1;
        }
       
        .gallery-overlay i {
            color: white;
            font-size: 2rem;
        }
       
        /* Reports Section */
        .reports-container {
            margin-top: 20px;
        }
       
        .reports-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
       
        .report-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
       
        .report-table th, .report-table td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: left;
        }
       
        .report-table th {
            background-color: #004d40;
            color: white;
        }
       
        .report-table tr:nth-child(even) {
            background-color: #f9f9f9;
        }
        
        .program-details {
            margin-top: 20px;
            padding: 20px;
            background-color: #f1fdfa;
            border-radius: 10px;
            border-left: 5px solid #004d40;
        }
        
        .program-details h3 {
            color: #004d40;
            margin-bottom: 15px;
        }
        
        .program-details p {
            margin-bottom: 10px;
        }
        
        .program-results {
            margin-top: 15px;
            padding: 15px;
            background-color: white;
            border-radius: 8px;
            border: 1px solid #ddd;
        }
        
        .program-results h4 {
            color: #004d40;
            margin-bottom: 10px;
        }
        
        .winner-list {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 15px;
        }
        
        .winner-item {
            text-align: center;
            padding: 10px;
            background-color: #f9f9f9;
            border-radius: 8px;
            min-width: 120px;
        }
        
        .winner-rank {
            font-weight: bold;
            color: #004d40;
            margin-bottom: 5px;
        }
        
        .winner-name {
            color: #333;
        }
       
        /* Members Section */
        .members-container {
            margin-top: 20px;
        }
        
        .members-part-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 20px;
        }
        
        .btn-part {
            background-color: #004d40;
            color: white;
            border: none;
            padding: 10px 25px;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
        }
        
        .btn-part:hover, .btn-part.active {
            background-color: #00796b;
            transform: translateY(-2px);
        }
        
        .part-indicator {
            text-align: center;
            margin-bottom: 15px;
            color: #004d40;
            font-weight: 600;
            font-size: 1.1rem;
        }
       
        .search-container {
            margin-bottom: 20px;
            text-align: center;
        }
       
        .search-input {
            width: 100%;
            max-width: 500px;
            padding: 12px 20px;
            border: 2px solid #004d40;
            border-radius: 50px;
            font-size: 1rem;
            outline: none;
        }
       
        .members-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }
       
        .member-card {
            background-color: #f1fdfa;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            cursor: pointer;
        }
       
        .member-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0,0,0,0.15);
        }
       
        .member-avatar {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            margin: 0 auto 15px;
            object-fit: cover;
            border: 3px solid #004d40;
        }
       
        .member-name {
            font-weight: 600;
            color: #004d40;
            margin-bottom: 5px;
        }
       
        .member-details {
            font-size: 0.9rem;
            color: #666;
        }
       
        .member-actions {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 15px;
        }
       
        .member-actions button {
            padding: 6px 12px;
            border-radius: 5px;
            font-size: 0.9rem;
            cursor: pointer;
            border: none;
            transition: all 0.3s ease;
        }
       
        .member-actions .btn-view {
            background-color: #004d40;
            color: white;
        }
       
        .member-actions .btn-view:hover {
            background-color: #00796b;
        }
       
        .member-actions .btn-fine {
            background-color: #e74c3c;
            color: white;
        }
       
        .member-actions .btn-fine:hover {
            background-color: #c0392b;
        }
       
        /* Awards Section */
        .awards-container {
            margin-top: 20px;
        }
        
        .results-tabs {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }
        
        .result-tab {
            background-color: #004d40;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .result-tab:hover, .result-tab.active {
            background-color: #00796b;
        }
        
        .results-content {
            display: none;
        }
        
        .results-content.active {
            display: block;
        }
        
        .program-result-card {
            background-color: #f1fdfa;
            border-radius: 10px;
            padding: 25px;
            margin-bottom: 20px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }
        
        .program-result-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            border-bottom: 2px solid #e0e0e0;
            padding-bottom: 15px;
        }
        
        .program-result-title {
            font-size: 1.4rem;
            color: #004d40;
            font-weight: 600;
        }
        
        .program-result-date {
            color: #666;
            font-size: 0.9rem;
        }
        
        .program-result-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-bottom: 20px;
        }
        
        .program-result-item {
            text-align: center;
            padding: 15px;
            background-color: white;
            border-radius: 8px;
            border: 1px solid #e0e0e0;
        }
        
        .program-result-item-label {
            font-size: 0.9rem;
            color: #666;
            margin-bottom: 5px;
        }
        
        .program-result-item-value {
            font-size: 1.2rem;
            font-weight: 600;
            color: #004d40;
        }
        
        .program-winners {
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            border: 1px solid #e0e0e0;
        }
        
        .program-winners h4 {
            color: #004d40;
            margin-bottom: 15px;
            font-size: 1.1rem;
        }
        
        .winner-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
        }
        
        .winner-card {
            text-align: center;
            padding: 15px;
            background-color: #f9f9f9;
            border-radius: 8px;
            transition: transform 0.3s ease;
        }
        
        .winner-card:hover {
            transform: translateY(-5px);
        }
        
        .winner-medal {
            font-size: 2rem;
            margin-bottom: 10px;
        }
        
        .winner-medal.first {
            color: #ffd700;
        }
        
        .winner-medal.second {
            color: #c0c0c0;
        }
        
        .winner-medal.third {
            color: #cd7f32;
        }
        
        .winner-card-name {
            font-weight: 600;
            color: #333;
            margin-bottom: 5px;
        }
        
        .winner-card-wing {
            font-size: 0.8rem;
            color: #666;
        }
       
        /* Library Section */
        .library-container {
            margin-top: 20px;
        }
        
        .library-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .library-search {
            margin-bottom: 20px;
        }
        
        .library-search input {
            width: 100%;
            max-width: 500px;
            padding: 12px 20px;
            border: 2px solid #004d40;
            border-radius: 50px;
            font-size: 1rem;
            outline: none;
        }
        
        .books-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .book-card {
            background-color: #f1fdfa;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }
        
        .book-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0,0,0,0.15);
        }
        
        .book-cover {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px;
            margin-bottom: 15px;
        }
        
        .book-title {
            font-size: 1.2rem;
            font-weight: 600;
            color: #004d40;
            margin-bottom: 10px;
        }
        
        .book-details {
            margin-bottom: 5px;
            color: #666;
        }
        
        .book-status {
            display: inline-block;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
            margin-top: 10px;
        }
        
        .book-status.available {
            background-color: #e8f5e9;
            color: #2e7d32;
        }
        
        .book-status.issued {
            background-color: #fff3e0;
            color: #ef6c00;
        }
        
        .book-status.reserved {
            background-color: #e3f2fd;
            color: #1565c0;
        }
        
        .book-actions {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }
        
        .book-actions button {
            flex: 1;
            padding: 8px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        
        .book-actions .btn-issue {
            background-color: #004d40;
            color: white;
        }
        
        .book-actions .btn-issue:hover {
            background-color: #00796b;
        }
        
        .book-actions .btn-reserve {
            background-color: #1565c0;
            color: white;
        }
        
        .book-actions .btn-reserve:hover {
            background-color: #1976d2;
        }
        
        .book-actions .btn-return {
            background-color: #ef6c00;
            color: white;
        }
        
        .book-actions .btn-return:hover {
            background-color: #f57c00;
        }
        
        .book-actions .btn-edit {
            background-color: #6a1b9a;
            color: white;
        }
        
        .book-actions .btn-edit:hover {
            background-color: #7b1fa2;
        }
        
        .book-actions .btn-delete {
            background-color: #c62828;
            color: white;
        }
        
        .book-actions .btn-delete:hover {
            background-color: #d32f2f;
        }
       
        /* Login Form */
        .login-container {
            max-width: 400px;
            margin: 0 auto;
            background-color: #f1fdfa;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            text-align: center;
        }
       
        .login-title {
            color: #004d40;
            margin-bottom: 20px;
            font-size: 1.8rem;
        }
       
        .login-form {
            text-align: left;
        }
       
        .form-group {
            margin-bottom: 20px;
        }
       
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: #004d40;
        }
       
        .form-group input {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
       
        .login-btn {
            background-color: #004d40;
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s ease;
            width: 100%;
        }
       
        .login-btn:hover {
            background-color: #00796b;
        }
       
        /* Member Profile Section */
        .profile-container {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 30px;
            margin-top: 20px;
        }
       
        .profile-sidebar {
            background-color: #f1fdfa;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }
       
        .profile-avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            margin: 0 auto 20px;
            object-fit: cover;
            border: 5px solid #004d40;
        }
       
        .profile-info {
            background-color: white;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }
       
        .profile-info h3 {
            color: #004d40;
            margin-bottom: 15px;
            font-size: 1.5rem;
            border-bottom: 2px solid #f1fdfa;
            padding-bottom: 10px;
        }
       
        .info-item {
            margin-bottom: 15px;
        }
       
        .info-label {
            font-weight: 600;
            color: #004d40;
            margin-bottom: 5px;
        }
       
        .info-value {
            color: #666;
        }
       
        .profile-actions {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }
       
        .profile-actions button {
            padding: 10px 20px;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            border: none;
            transition: all 0.3s ease;
        }
       
        .profile-actions .btn-fine {
            background-color: #e74c3c;
            color: white;
        }
       
        .profile-actions .btn-fine:hover {
            background-color: #c0392b;
        }
       
        .profile-actions .btn-back {
            background-color: #7f8c8d;
            color: white;
        }
       
        .profile-actions .btn-back:hover {
            background-color: #636e72;
        }
       
        /* Fine Section */
        .fine-container {
            max-width: 600px;
            margin: 0 auto;
            background-color: #f1fdfa;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
       
        .fine-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            border-bottom: 2px solid #004d40;
            padding-bottom: 15px;
        }
       
        .fine-header h3 {
            color: #004d40;
            font-size: 1.5rem;
        }
       
        .fine-back {
            background-color: #7f8c8d;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
       
        .fine-back:hover {
            background-color: #636e72;
        }
       
        .fine-form {
            margin-top: 20px;
        }
       
        .fine-actions {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }
       
        .fine-actions button {
            padding: 10px 20px;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            border: none;
            transition: all 0.3s ease;
        }
       
        .fine-actions .btn-submit {
            background-color: #004d40;
            color: white;
        }
       
        .fine-actions .btn-submit:hover {
            background-color: #00796b;
        }
       
        .fine-actions .btn-cancel {
            background-color: #e74c3c;
            color: white;
        }
       
        .fine-actions .btn-cancel:hover {
            background-color: #c0392b;
        }
        
        /* Fine Status Card */
        .fine-status-card {
            background-color: #fff8e1;
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 20px;
            border-left: 5px solid #ffc107;
        }
        
        .fine-status-card h3 {
            color: #ff6f00;
            margin-bottom: 10px;
        }
        
        .fine-status-card p {
            color: #555;
        }
        
        .fine-status-card .fine-amount {
            font-size: 1.5rem;
            font-weight: bold;
            color: #e74c3c;
            margin: 10px 0;
        }
        
        .fine-status-card .no-fine {
            color: #4caf50;
            font-weight: bold;
        }
       
        /* Cash Payment Section */
        .cash-container {
            max-width: 600px;
            margin: 0 auto;
            background-color: #f1fdfa;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
       
        .cash-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            border-bottom: 2px solid #004d40;
            padding-bottom: 15px;
        }
       
        .cash-header h3 {
            color: #004d40;
            font-size: 1.5rem;
        }
       
        .cash-back {
            background-color: #7f8c8d;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
       
        .cash-back:hover {
            background-color: #636e72;
        }
       
        .cash-form {
            margin-top: 20px;
        }
       
        .cash-actions {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }
       
        .cash-actions button {
            padding: 10px 20px;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            border: none;
            transition: all 0.3s ease;
        }
       
        .cash-actions .btn-submit {
            background-color: #004d40;
            color: white;
        }
       
        .cash-actions .btn-submit:hover {
            background-color: #00796b;
        }
       
        .cash-actions .btn-cancel {
            background-color: #e74c3c;
            color: white;
        }
       
        .cash-actions .btn-cancel:hover {
            background-color: #c0392b;
        }
        
        .cash-amount {
            font-size: 1.5rem;
            font-weight: bold;
            color: #e74c3c;
            margin: 10px 0;
        }
       
        /* Footer */
        footer {
            background-color: #004d40;
            color: white;
            padding: 40px 0 20px;
            margin-top: 40px;
        }
       
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
       
        .footer-column h3 {
            color: #ffd54f;
            margin-bottom: 20px;
            font-size: 1.3rem;
        }
       
        .footer-links {
            list-style: none;
        }
       
        .footer-links li {
            margin-bottom: 10px;
        }
       
        .footer-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s ease;
        }
       
        .footer-links a:hover {
            color: #ffd54f;
        }
       
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
       
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            transition: all 0.3s ease;
        }
       
        .social-links a:hover {
            background-color: #ffd54f;
            color: #004d40;
        }
       
        .copyright {
            text-align: center;
            padding-top: 20px;
            margin-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            color: #b2dfdb;
        }
       
        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1001;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.5);
            align-items: center;
            justify-content: center;
        }
       
        .modal-content {
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            max-width: 500px;
            width: 90%;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            animation: modalFadeIn 0.3s;
        }
       
        @keyframes modalFadeIn {
            from {opacity: 0; transform: translateY(-50px);}
            to {opacity: 1; transform: translateY(0);}
        }
       
        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            border-bottom: 2px solid #f1fdfa;
            padding-bottom: 15px;
        }
       
        .modal-title {
            color: #004d40;
            font-size: 1.5rem;
            font-weight: 600;
        }
       
        .close-modal {
            font-size: 1.5rem;
            cursor: pointer;
            color: #666;
            transition: color 0.3s;
        }
       
        .close-modal:hover {
            color: #e74c3c;
        }
       
        .modal-form {
            display: grid;
            gap: 15px;
        }
       
        .form-group {
            margin-bottom: 15px;
        }
       
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: #004d40;
        }
       
        .form-group input, .form-group select, .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
       
        .form-group textarea {
            resize: vertical;
            min-height: 80px;
        }
       
        .modal-footer {
            display: flex;
            justify-content: flex-end;
            gap: 10px;
            margin-top: 20px;
        }
       
        .btn-cancel {
            background-color: #e74c3c;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
       
        .btn-cancel:hover {
            background-color: #c0392b;
        }
        
        .btn-confirm {
            background-color: #004d40;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        .btn-confirm:hover {
            background-color: #00796b;
        }
       
        /* Admin Dashboard Styles */
        .admin-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }
       
        .admin-card {
            background-color: #f1fdfa;
            border-radius: 10px;
            padding: 25px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s ease;
        }
       
        .admin-card:hover {
            transform: translateY(-5px);
        }
       
        .admin-card i {
            font-size: 3rem;
            color: #004d40;
            margin-bottom: 20px;
        }
       
        .admin-card h3 {
            color: #004d40;
            margin-bottom: 15px;
            font-size: 1.4rem;
        }
       
        /* Member Selection Modal Styles */
        .member-selection-card {
            background-color: #f1fdfa;
            border-radius: 10px;
            padding: 15px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .member-selection-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0,0,0,0.15);
        }
        
        .member-selection-card.selected {
            border: 2px solid #004d40;
            background-color: #e8f5e9;
        }
        
        .member-selection-avatar {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            margin: 0 auto 10px;
            object-fit: cover;
            border: 2px solid #004d40;
        }
        
        .member-selection-name {
            font-weight: 600;
            color: #004d40;
            margin-bottom: 5px;
        }
        
        .member-selection-admission {
            font-size: 0.8rem;
            color: #666;
            margin-bottom: 10px;
        }
        
        .member-selection-actions {
            display: flex;
            justify-content: center;
        }
        
        .member-selection-actions button {
            padding: 5px 10px;
            border-radius: 5px;
            font-size: 0.8rem;
            cursor: pointer;
            border: none;
            transition: all 0.3s ease;
            background-color: #004d40;
            color: white;
        }
        
        .member-selection-actions button:hover {
            background-color: #00796b;
        }
        
        .modal-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 15px;
            max-height: 400px;
            overflow-y: auto;
            margin: 15px 0;
        }
        
        .modal-search {
            margin-bottom: 15px;
        }
        
        .modal-search input {
            width: 100%;
            padding: 10px 15px;
            border: 2px solid #004d40;
            border-radius: 50px;
            font-size: 1rem;
            outline: none;
        }
       
        /* Responsive Styles */
        @media (max-width: 768px) {
            nav {
                display: none;
            }
            
            .header-container {
                flex-direction: column;
                gap: 15px;
            }
            
            .user-actions {
                width: 100%;
                justify-content: center;
            }
            
            .profile-container {
                grid-template-columns: 1fr;
            }
            
            .gallery-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .members-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .books-grid {
                grid-template-columns: repeat(1, 1fr);
            }
            
            .award-winners {
                flex-direction: column;
                gap: 15px;
            }
            
            .members-part-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .library-header {
                flex-direction: column;
                gap: 15px;
            }
            
            .results-tabs {
                flex-direction: column;
                align-items: center;
            }
            
            .program-result-header {
                flex-direction: column;
                gap: 10px;
                text-align: center;
            }
            
            .winner-grid {
                grid-template-columns: repeat(1, 1fr);
            }
            
            .report-table {
                font-size: 0.9rem;
            }
            
            .report-table th, .report-table td {
                padding: 8px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="header-container">
            <div class="logo">
                <img src="https://i.ibb.co/9mTqW06s/mail-google.png" alt="mail-google" border="0">
                <h1>USWA 40th Batch</h1>
            </div>
            <nav>
                <a href="#" class="active" onclick="showSection('home')">Home</a>
                <a href="#" onclick="showSection('about')">About Us</a>
                <a href="#" onclick="showSection('gallery')">Gallery</a>
                <a href="#" onclick="showSection('reports')">Reports</a>
                <a href="#" onclick="showSection('awards')">Results</a>
                <a href="#" onclick="showSection('members')">Members</a>
                <a href="#" onclick="showSection('library')">Library</a>
                <a href="#" onclick="showSection('contact')">Contact</a>
            </nav>
            <div class="user-actions">
                <a href="#" class="btn btn-outline" onclick="showSection('login')">Login</a>
                <a href="#" class="btn btn-primary">Apply Now</a>
                <button id="logoutBtn" class="btn-logout" onclick="logout()" style="display: none;">Logout</button>
            </div>
        </div>
    </header>
    
    <main>
        <!-- Home Section -->
        <section id="home" class="section active">
            <div class="hero">
                <h2>Welcome to Uswa 40th Batch</h2>
                <p>Your journey to knowledge and spiritual growth begins here. We provide a comprehensive Islamic education with modern academic excellence.</p>
                <a href="#" class="btn btn-primary">Explore Programs</a>
            </div>
           
            <div class="section-title">
                <h2>Why Choose Darul Huda?</h2>
                <p>Providing excellence in Islamic education for over two decades</p>
            </div>
           
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-graduation-cap"></i>
                    </div>
                    <div class="feature-content">
                        <h3>Academic Excellence</h3>
                        <p>We strive for academic excellence through rigorous curriculum and dedicated teaching.</p>
                    </div>
                </div>
               
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-hands-helping"></i>
                    </div>
                    <div class="feature-content">
                        <h3>Community Service</h3>
                        <p>We engage in community service projects to benefit society and develop leadership skills.</p>
                    </div>
                </div>
               
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-mosque"></i>
                    </div>
                    <div class="feature-content">
                        <h3>Islamic Values</h3>
                        <p>We uphold Islamic values and ethics in all our activities and decision-making.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- About Section -->
        <section id="about" class="section">
            <div class="section-title">
                <h2>About Us</h2>
                <p>Learn about our mission, vision, and values</p>
            </div>
            <p style="text-align: center; margin-bottom: 30px; font-size: 1.1rem;">
                The Uswa 40th batch represents a vibrant community of dedicated students at Darul Huda Islamic University, 
                committed to excellence in both Islamic and contemporary education.
            </p>
           
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-graduation-cap"></i>
                    </div>
                    <div class="feature-content">
                        <h3>Academic Excellence</h3>
                        <p>We strive for academic excellence through rigorous curriculum and dedicated teaching.</p>
                    </div>
                </div>
               
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-hands-helping"></i>
                    </div>
                    <div class="feature-content">
                        <h3>Community Service</h3>
                        <p>We engage in community service projects to benefit society and develop leadership skills.</p>
                    </div>
                </div>
               
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-mosque"></i>
                    </div>
                    <div class="feature-content">
                        <h3>Islamic Values</h3>
                        <p>We uphold Islamic values and ethics in all our activities and decision-making.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Gallery Section -->
        <section id="gallery" class="section">
            <div class="section-title">
                <h2>Gallery</h2>
                <p>Capturing moments from our journey</p>
            </div>
           
            <div class="gallery-grid">
                <div class="gallery-item">
                    <img src="https://i.ibb.co/bgC4c7qX/unnamed.jpg" alt="Batch Activity">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://i.ibb.co/dsrX5fXr/unnamed.jpg" alt="Classroom">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://i.ibb.co/ycYTgz0c/unnamed.jpg" alt="Students">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://i.ibb.co/nsq8gnPX/unnamed.jpg" alt="Event">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://i.ibb.co/rRcn7MdY/unnamed.jpg" alt="Campus">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://i.ibb.co/9mKzTG7h/unnamed.jpg" alt="Campus">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://i.ibb.co/qfyDzbH/unnamed.jpg" alt="Study Group">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Reports Section -->
        <section id="reports" class="section">
            <div class="section-title">
                <h2>Reports</h2>
                <p>Program reports and activities</p>
            </div>
           
            <div class="reports-container">
                <div class="reports-header">
                    <button class="btn-success" onclick="openAddReportModal()">
                        <i class="fas fa-plus"></i> Add Report
                    </button>
                </div>
               
                <div id="reportsContent">
                    <!-- Reports content will be dynamically generated here -->
                </div>
            </div>
        </section>
        
        <!-- Awards Section -->
        <section id="awards" class="section">
            <div class="section-title">
                <h2>Results</h2>
                <p>Achievements and awards of our students</p>
            </div>
            
            <div class="results-tabs">
                <button class="result-tab active" onclick="showResults('all')">All Programs</button>
                <button class="result-tab" onclick="showResults('english')">English Wing</button>
                <button class="result-tab" onclick="showResults('arabic')">Arabic Wing</button>
                <button class="result-tab" onclick="showResults('acadamic')">Academic Wing</button>
                <button class="result-tab" onclick="showResults('urdu')">Urdu Wing</button>
                <button class="result-tab" onclick="showResults('malayalam')">Malayalam Wing</button>
                <button class="result-tab" onclick="showResults('library')">Library Wing</button>
            </div>
            
            <div id="allResults" class="results-content active">
                <!-- All results will be displayed here -->
            </div>
            
            <div id="englishResults" class="results-content">
                <!-- English wing results will be displayed here -->
            </div>
            
            <div id="arabicResults" class="results-content">
                <!-- Arabic wing results will be displayed here -->
            </div>
            
            <div id="acadamicResults" class="results-content">
                <!-- Academic wing results will be displayed here -->
            </div>
            
            <div id="urduResults" class="results-content">
                <!-- Urdu wing results will be displayed here -->
            </div>
            
            <div id="malayalamResults" class="results-content">
                <!-- Malayalam wing results will be displayed here -->
            </div>
            
            <div id="libraryResults" class="results-content">
                <!-- Library wing results will be displayed here -->
            </div>
        </section>
        
        <!-- Members Section -->
        <section id="members" class="section">
            <div class="section-title">
                <h2>Members</h2>
                <p>Our dedicated team of student representatives</p>
            </div>
            
            <div class="members-container">
                <div class="members-part-buttons">
                    <button class="btn-part active" onclick="showMembersPart(1)">2-A</button>
                    <button class="btn-part" onclick="showMembersPart(2)">2-B</button>
                </div>
                
                <div class="part-indicator" id="partIndicator">Showing 2-A</div>
                
                <div class="search-container">
                    <input type="text" id="memberSearch" class="search-input" placeholder="Search members by name..." oninput="filterMembers()">
                </div>
                
                <div class="members-grid" id="membersContainer">
                    <!-- Member cards will be dynamically generated here -->
                </div>
            </div>
        </section>
        
        <!-- Library Section -->
        <section id="library" class="section">
            <div class="section-title">
                <h2>Library</h2>
                <p>Explore our collection of books and resources</p>
            </div>
            
            <div class="library-container">
                <div class="library-header">
                    <div class="library-search">
                        <input type="text" id="bookSearch" class="search-input" placeholder="Search books by title, author, or ISBN..." oninput="filterBooks()">
                    </div>
                    <button class="btn-success" onclick="openAddBookModal()">
                        <i class="fas fa-plus"></i> Add Book
                    </button>
                </div>
                
                <div class="books-grid" id="booksContainer">
                    <!-- Book cards will be dynamically generated here -->
                </div>
            </div>
        </section>
        
        <!-- Contact Section -->
        <section id="contact" class="section">
            <div class="section-title">
                <h2>Contact Us</h2>
                <p>We're here to help with any questions or concerns</p>
            </div>
           
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px;">
                <div style="background-color: #f1fdfa; padding: 25px; border-radius: 10px; box-shadow: 0 3px 10px rgba(0,0,0,0.1);">
                    <h3 style="color: #004d40; margin-bottom: 20px; text-align: center;">Visit Us</h3>
                    <p style="margin-bottom: 15px;"><i class="fas fa-map-marker-alt" style="color: #004d40; margin-right: 10px;"></i> Darul Huda Islamic University, Panakkad, Malappuram, Kerala</p>
                    <p style="margin-bottom: 15px;"><i class="fas fa-phone" style="color: #004d40; margin-right: 10px;"></i> +91-483-274-2345</p>
                    <p><i class="fas fa-envelope" style="color: #004d40; margin-right: 10px;"></i> uswafriends2024@gmail.com</p>
                </div>
               
                <div style="background-color: #f1fdfa; padding: 25px; border-radius: 10px; box-shadow: 0 3px 10px rgba(0,0,0,0.1);">
                    <h3 style="color: #004d40; margin-bottom: 20px; text-align: center;">Mobile</h3>
                    <p style="margin-bottom: 15px;"><i class="fas fa-user-friends" style="color: #004d40; margin-right: 10px;"></i> Student Affairs: +91-483-274-2346</p>
                    <p style="margin-bottom: 15px;"><i class="fas fa-book" style="color: #004d40; margin-right: 10px;"></i> Library: +91-483-274-2350</p>
                    <p><i class="fas fa-graduation-cap" style="color: #004d40; margin-right: 10px;"></i> Batch phone: +91-483-274-2348</p>
                </div>
            </div>
        </section>
        
        <!-- Login Section -->
        <section id="login" class="section">
            <div class="login-container">
                <h2 class="login-title">Student Login</h2>
                <form class="login-form">
                    <div class="form-group">
                        <label for="username">Username</label>
                        <input type="text" id="username" placeholder="Enter your username">
                    </div>
                    <div class="form-group">
                        <label for="password">Password</label>
                        <input type="password" id="password" placeholder="Enter your password">
                    </div>
                    <button type="button" class="login-btn" onclick="attemptLogin()">Login</button>
                </form>
            </div>
        </section>
        
        <!-- Admin Login Section -->
        <section id="adminLogin" class="section">
            <div class="login-container">
                <h2 class="login-title">Admin Login</h2>
                <form class="login-form">
                    <div class="form-group">
                        <label for="adminUsername">Admin Username</label>
                        <input type="text" id="adminUsername" placeholder="Enter admin username">
                    </div>
                    <div class="form-group">
                        <label for="adminPassword">Admin Password</label>
                        <input type="password" id="adminPassword" placeholder="Enter admin password">
                    </div>
                    <button type="button" class="login-btn" onclick="attemptAdminLogin()">Admin Login</button>
                </form>
            </div>
        </section>
        
        <!-- Admin Home Section -->
        <section id="adminHome" class="section">
            <div class="section-title">
                <h2>Admin Dashboard</h2>
                <p>Manage library fines and cash payments</p>
            </div>
            <div class="admin-cards">
                <div class="admin-card">
                    <i class="fas fa-plus-circle"></i>
                    <h3>Add Fine</h3>
                    <p>Add library fines to student accounts</p>
                    <button class="btn-success" onclick="openMembersSelectionModal('addFine')">Add Fine</button>
                </div>
                <div class="admin-card">
                    <i class="fas fa-money-bill-wave"></i>
                    <h3>Process Cash</h3>
                    <p>Process cash payments from students</p>
                    <button class="btn-success" onclick="openMembersSelectionModal('processCash')">Process Cash</button>
                </div>
                <div class="admin-card">
                    <i class="fas fa-users"></i>
                    <h3>View Members</h3>
                    <p>Search and view member details</p>
                    <button class="btn-success" onclick="showSection('members')">View Members</button>
                </div>
                <div class="admin-card">
                    <i class="fas fa-book-reader"></i>
                    <h3>Library Books</h3>
                    <p>Check book status and manage library records</p>
                    <button class="btn-success" onclick="showSection('library')">Manage Books</button>
                </div>
            </div>
        </section>
        
        <!-- Member Profile Section -->
        <section id="profile" class="section">
            <div class="section-title">
                <h2>Member Profile</h2>
                <p>View detailed information about members</p>
            </div>
            
            <!-- Fine Status Card -->
            <div class="fine-status-card" id="fineStatusCard">
                <h3>Library Fine Status</h3>
                <div id="fineStatusContent">
                    <div class="fine-amount" id="profileFineAmount">₹0</div>
                    <p id="profileFineMessage">No pending fines</p>
                </div>
            </div>
            
            <div class="profile-container">
                <div class="profile-sidebar">
                    <img id="profileAvatar" class="profile-avatar" src="" alt="Profile Picture">
                    <h3 id="profileName" class="member-name"></h3>
                    <div class="member-details" id="profileAdmissionNo"></div>
                </div>
                <div class="profile-info">
                    <h3>Student Details</h3>
                    <div class="info-item">
                        <div class="info-label">Mobile Number</div>
                        <div class="info-value" id="profileMobile"></div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Date of Birth</div>
                        <div class="info-value" id="profileDob"></div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Rank</div>
                        <div class="info-value" id="profileRank"></div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Currently Studying</div>
                        <div class="info-value" id="profileStudying"></div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Library Status</div>
                        <div class="info-value" id="profileLibraryStatus"></div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Books Issued</div>
                        <div class="info-value" id="profileBooksIssued"></div>
                    </div>
                    <div class="info-item">
                        <div class="info-label">Library Fine</div>
                        <div class="info-value" id="profileLibraryFine"></div>
                    </div>
                    <div class="profile-actions">
                        <button class="btn-fine" onclick="openAddFineModal()" id="addFineBtn">Add Fine</button>
                        <button class="btn-fine" onclick="openRemoveFineModal()" id="removeFineBtn">Remove Fine</button>
                        <button class="btn-fine" onclick="openCashModal()">Pay Cash to Admin</button>
                        <button class="btn-back" onclick="showSection('members')">Back to Members</button>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Fine Section -->
        <section id="fine" class="section">
            <div class="fine-container">
                <div class="fine-header">
                    <h3>Library Fine Details</h3>
                    <button class="fine-back" onclick="showSection('profile')">Back to Profile</button>
                </div>
                <div class="info-item">
                    <div class="info-label">Student Name</div>
                    <div class="info-value" id="fineName"></div>
                </div>
                <div class="info-item">
                    <div class="info-label">Admission Number</div>
                    <div class="info-value" id="fineAdmissionNo"></div>
                </div>
                <div class="info-item">
                    <div class="info-label">Fine Amount</div>
                    <div class="info-value" id="fineAmount"></div>
                </div>
                <div class="info-item">
                    <div class="info-label">Reason</div>
                    <div class="info-value" id="fineReason"></div>
                </div>
                <div class="info-item">
                    <div class="info-label">Status</div>
                    <div class="info-value" id="fineStatus"></div>
                </div>
                <div class="fine-actions">
                    <button class="btn-submit" onclick="payFine()">Pay Fine</button>
                    <button class="btn-cancel" onclick="showSection('profile')">Cancel</button>
                </div>
            </div>
        </section>
        
        <!-- Cash Payment Section -->
        <section id="cash" class="section">
            <div class="cash-container">
                <div class="cash-header">
                    <h3>Cash Payment to Admin</h3>
                    <button class="cash-back" onclick="showSection('profile')">Back to Profile</button>
                </div>
                <div class="info-item">
                    <div class="info-label">Student Name</div>
                    <div class="info-value" id="cashName"></div>
                </div>
                <div class="info-item">
                    <div class="info-label">Admission Number</div>
                    <div class="info-value" id="cashAdmissionNo"></div>
                </div>
                <div class="info-item">
                    <div class="info-label">Payment Type</div>
                    <div class="info-value">Cash</div>
                </div>
                <div class="info-item">
                    <div class="info-label">Recipient</div>
                    <div class="info-value">Admin</div>
                </div>
                <div class="info-item">
                    <div class="info-label">Amount</div>
                    <div class="cash-amount" id="cashAmount">₹0</div>
                </div>
                <div class="info-item">
                    <div class="info-label">Reason</div>
                    <div class="info-value" id="cashReason">Library Fine Payment</div>
                </div>
                <div class="cash-actions">
                    <button class="btn-submit" onclick="processCashPayment()">Process Payment</button>
                    <button class="btn-cancel" onclick="showSection('profile')">Cancel</button>
                </div>
            </div>
        </section>
    </main>
    
    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-column">
                <h3>Darul Huda</h3>
                <p>Providing excellence in Islamic education since 2000</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-facebook-f"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-youtube"></i></a>
                </div>
            </div>
           
            <div class="footer-column">
                <h3>Quick Links</h3>
                <ul class="footer-links">
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About Us</a></li>
                    <li><a href="#">Academics</a></li>
                    <li><a href="#">Admissions</a></li>
                    <li><a href="#">Campus Life</a></li>
                </ul>
            </div>
           
            <div class="footer-column">
                <h3>Resources</h3>
                <ul class="footer-links">
                    <li><a href="#">Library</a></li>
                    <li><a href="#">E-Learning</a></li>
                    <li><a href="#">Academic Calendar</a></li>
                    <li><a href="#">Syllabus</a></li>
                    <li><a href="#">Examinations</a></li>
                </ul>
            </div>
           
            <div class="footer-column">
                <h3>Contact Information</h3>
                <ul class="footer-links">
                    <li><i class="fas fa-map-marker-alt"></i> Darul Huda Islamic University, Chemmad, Malappuram, Kerala</li>
                    <li><i class="fas fa-phone"></i> +91-483-274-2345</li>
                    <li><i class="fas fa-envelope"></i> uswafriends2024@gmail.com</li>
                </ul>
            </div>
        </div>
       
        <div class="copyright">
            &copy; 2023 Darul Huda Islamic University. All Rights Reserved.
        </div>
    </footer>
   
    <!-- Modal Styles -->
    <div id="addReportModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3 class="modal-title">Add New Report</h3>
                <span class="close-modal" onclick="closeAddReportModal()">&times;</span>
            </div>
            <form class="modal-form" id="addReportForm">
                <div class="form-group">
                    <label for="programName">Program Name</label>
                    <input type="text" id="programName" placeholder="Enter program name" required>
                </div>
                <div class="form-group">
                    <label for="programDate">Date</label>
                    <input type="date" id="programDate" required>
                </div>
                <div class="form-group">
                    <label for="participation">Participation</label>
                    <input type="number" id="participation" placeholder="Number of participants" min="1" required>
                </div>
                <div class="form-group">
                    <label for="remarks">Remarks</label>
                    <select id="remarks" required>
                        <option value="">Select remarks</option>
                        <option value="Excellent">Excellent</option>
                        <option value="Very Good">Very Good</option>
                        <option value="Good">Good</option>
                        <option value="Average">Average</option>
                        <option value="Poor">Poor</option>
                    </select>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn-cancel" onclick="closeAddReportModal()">Cancel</button>
                    <button type="button" class="btn-success" onclick="addReport()">Add Report</button>
                </div>
            </form>
        </div>
    </div>
   
    <!-- View Profile Modal -->
    <div id="viewProfileModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3 class="modal-title">Login to View Profile</h3>
                <span class="close-modal" onclick="closeViewProfileModal()">&times;</span>
            </div>
            <form class="modal-form" id="viewProfileForm">
                <div class="form-group">
                    <label for="profileUsername">Username</label>
                    <input type="text" id="profileUsername" placeholder="Enter your username" required>
                </div>
                <div class="form-group">
                    <label for="profilePassword">Password</label>
                    <input type="password" id="profilePassword" placeholder="Enter your password" required>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn-cancel" onclick="closeViewProfileModal()">Cancel</button>
                    <button type="button" class="btn-success" onclick="viewProfile()">View Profile</button>
                </div>
            </form>
        </div>
    </div>
   
    <!-- Add Fine Modal -->
    <div id="addFineModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3 class="modal-title">Add Library Fine</h3>
                <span class="close-modal" onclick="closeAddFineModal()">&times;</span>
            </div>
            <form class="modal-form" id="addFineForm">
                <div class="form-group">
                    <label for="addFineAmount">Fine Amount (₹)</label>
                    <input type="number" id="addFineAmount" placeholder="Enter fine amount" min="1" required>
                </div>
                <div class="form-group">
                    <label for="addFineReason">Reason</label>
                    <select id="addFineReason" required>
                        <option value="">Select reason</option>
                        <option value="Late Return">Late Return</option>
                        <option value="Damaged Book">Damaged Book</option>
                        <option value="Lost Book">Lost Book</option>
                        <option value="Other">Other</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="addFineNotes">Notes (Optional)</label>
                    <textarea id="addFineNotes" placeholder="Additional details about the fine"></textarea>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn-cancel" onclick="closeAddFineModal()">Cancel</button>
                    <button type="button" class="btn-success" onclick="addFine()">Add Fine</button>
                </div>
            </form>
        </div>
    </div>
   
    <!-- Remove Fine Modal -->
    <div id="removeFineModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3 class="modal-title">Remove Library Fine</h3>
                <span class="close-modal" onclick="closeRemoveFineModal()">&times;</span>
            </div>
            <form class="modal-form" id="removeFineForm">
                <div class="form-group">
                    <label for="removeFineAmount">Fine Amount to Remove (₹)</label>
                    <input type="number" id="removeFineAmount" placeholder="Enter amount to remove" min="1" required>
                </div>
                <div class="form-group">
                    <label for="removeReason">Reason</label>
                    <select id="removeReason" required>
                        <option value="">Select reason</option>
                        <option value="Correction">Correction</option>
                        <option value="Payment Received">Payment Received</option>
                        <option value="Mistake">Mistake</option>
                        <option value="Other">Other</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="removeNotes">Notes (Optional)</label>
                    <textarea id="removeNotes" placeholder="Additional details about the removal"></textarea>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn-cancel" onclick="closeRemoveFineModal()">Cancel</button>
                    <button type="button" class="btn-success" onclick="removeFine()">Remove Fine</button>
                </div>
            </form>
        </div>
    </div>
   
    <!-- Add Book Modal -->
    <div id="addBookModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3 class="modal-title">Add New Book</h3>
                <span class="close-modal" onclick="closeAddBookModal()">&times;</span>
            </div>
            <form class="modal-form" id="addBookForm">
                <div class="form-group">
                    <label for="bookTitle">Book Title</label>
                    <input type="text" id="bookTitle" placeholder="Enter book title" required>
                </div>
                <div class="form-group">
                    <label for="bookAuthor">Author</label>
                    <input type="text" id="bookAuthor" placeholder="Enter author name" required>
                </div>
                <div class="form-group">
                    <label for="bookISBN">ISBN</label>
                    <input type="text" id="bookISBN" placeholder="Enter ISBN number" required>
                </div>
                <div class="form-group">
                    <label for="bookGenre">Genre</label>
                    <select id="bookGenre" required>
                        <option value="">Select genre</option>
                        <option value="Islamic Studies">Islamic Studies</option>
                        <option value="Quran">Quran</option>
                        <option value="Hadith">Hadith</option>
                        <option value="Arabic Language">Arabic Language</option>
                        <option value="History">History</option>
                        <option value="Philosophy">Philosophy</option>
                        <option value="Science">Science</option>
                        <option value="Literature">Literature</option>
                        <option value="Other">Other</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="bookStatus">Status</label>
                    <select id="bookStatus" required>
                        <option value="available">Available</option>
                        <option value="issued">Issued</option>
                        <option value="reserved">Reserved</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="bookDescription">Description (Optional)</label>
                    <textarea id="bookDescription" placeholder="Enter book description"></textarea>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn-cancel" onclick="closeAddBookModal()">Cancel</button>
                    <button type="button" class="btn-success" onclick="addBook()">Add Book</button>
                </div>
            </form>
        </div>
    </div>
   
    <!-- Edit Book Modal -->
    <div id="editBookModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3 class="modal-title">Edit Book</h3>
                <span class="close-modal" onclick="closeEditBookModal()">&times;</span>
            </div>
            <form class="modal-form" id="editBookForm">
                <div class="form-group">
                    <label for="editBookTitle">Book Title</label>
                    <input type="text" id="editBookTitle" required>
                </div>
                <div class="form-group">
                    <label for="editBookAuthor">Author</label>
                    <input type="text" id="editBookAuthor" required>
                </div>
                <div class="form-group">
                    <label for="editBookISBN">ISBN</label>
                    <input type="text" id="editBookISBN" required>
                </div>
                <div class="form-group">
                    <label for="editBookGenre">Genre</label>
                    <select id="editBookGenre" required>
                        <option value="Islamic Studies">Islamic Studies</option>
                        <option value="Quran">Quran</option>
                        <option value="Hadith">Hadith</option>
                        <option value="Arabic Language">Arabic Language</option>
                        <option value="History">History</option>
                        <option value="Philosophy">Philosophy</option>
                        <option value="Science">Science</option>
                        <option value="Literature">Literature</option>
                        <option value="Other">Other</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="editBookStatus">Status</label>
                    <select id="editBookStatus" required>
                        <option value="available">Available</option>
                        <option value="issued">Issued</option>
                        <option value="reserved">Reserved</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="editBookDescription">Description (Optional)</label>
                    <textarea id="editBookDescription"></textarea>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn-cancel" onclick="closeEditBookModal()">Cancel</button>
                    <button type="button" class="btn-success" onclick="updateBook()">Update Book</button>
                </div>
            </form>
        </div>
    </div>
   
    <!-- Members Selection Modal -->
    <div id="membersSelectionModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h3 class="modal-title">Select a Member</h3>
                <span class="close-modal" onclick="closeMembersSelectionModal()">&times;</span>
            </div>
            <div class="modal-body">
                <div class="modal-search">
                    <input type="text" id="membersSearchInput" placeholder="Search members by name or admission number..." oninput="searchMembersSelection()">
                </div>
                <div class="modal-grid" id="membersSelectionGrid">
                    <!-- Member selection cards will be dynamically generated here -->
                </div>
            </div>
            <div class="modal-footer">
                <button class="btn-cancel" onclick="closeMembersSelectionModal()">Cancel</button>
                <button class="btn-confirm" onclick="confirmMemberSelection()">Confirm</button>
            </div>
        </div>
    </div>
    
    <script>
      // Members data array
        const members = [
            { name: "Rayyan.pk", username: "Rayyan.pk", password: "4051", photo: "https://i.ibb.co/231yXdbt/4051.jpg", mobile: "9784548325", dateOfBirth: "2-5-13", admissionNo: "4051", rank: "33", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Finan K", username: "Finan", password: "4040", photo: "https://i.ibb.co/wN8m9FZj/4040.jpg", mobile: "9784548325", dateOfBirth: "2-5-13", admissionNo: "4040", rank: "33", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Fasalu Rahman.k", username: "Fasalu", password: "4005", photo: "https://i.ibb.co/rn1vX70/unnamed.jpg", mobile: "9784548325", dateOfBirth: "2-5-13", admissionNo: "4005", rank: "29", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Thasneem Kt", username: "thasneem.kt", password: "4061", photo: "https://i.ibb.co/C3VRTQw2/4061.jpg", admissionNo: "4061", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Mk", username: "muhammed.mk", password: "4068", photo: "https://i.ibb.co/r2yMYvJd/4068.jpg", admissionNo: "4068", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Shaz P", username: "shaz.p", password: "4008", photo: "https://i.ibb.co/hFmzJ25B/unnamed.jpg", admissionNo: "4008", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Rajib Ek", username: "rajib.ek", password: "4017", photo: "https://i.ibb.co/CsHbMwFG/unnamed.jpg", admissionNo: "4017", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Ayman Abdussamad", username: "Ayman", password: "4075", photo: "https://i.ibb.co/C5FRkkMn/4075.jpg", admissionNo: "4075", studying: "Some University", semesterTopper: "2", campusTopper: "1 year", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "ABDUL RAHEEM M.P", username: "RAHEEM", password: "4074", photo: "https://i.ibb.co/tM5K1Tbc/4074.jpg", admissionNo: "4074", rank: "3" ,studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muzammil N.A", username: "Muzammil", password: "4081", photo: "https://i.ibb.co/8FpCTGf/4081.jpg", admissionNo: "4081", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Zayan K.V", username: "Zayan", password: "4067", photo: "https://i.ibb.co/mCHzKBc4/4067.jpg", admissionNo: "4067", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Radeef ", username: "Radeef", password: "4069", photo: "https://i.ibb.co/vxTb3yZ1/4069.jpg", admissionNo: "4069", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Rayyan E.K", username: "Rayyan E.K", password: "4052", photo: "https://i.ibb.co/gZcDTJdk/4052.jpg", admissionNo: "4052", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Shadhi P", username: "Shadhi", password: "4059", photo: "https://i.ibb.co/j9m21N16/4059.jpg", admissionNo: "4059", rank: "16" ,studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Ameen A.K", username: "Ameen.ak", password: "4073", photo: "https://i.ibb.co/RGBkGKgY/4073.jpg", admissionNo: "4073", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Sameeh K", username: "Sameeh", password: "4070", photo: "https://i.ibb.co/zWgDzNww/4070.jpg", admissionNo: "4070", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Shareef T", username: "Shareef", password: "4048", photo: "https://i.ibb.co/8DmBxTpB/4048.jpg", admissionNo: "4048", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Abdullah V.S", username: "Abdullah", password: "4080", photo: "https://i.ibb.co/pvhwWPTp/4080.jpg", admissionNo: "4080", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Ajuvad Ameen", username: "Ameen.p", password: "4058", photo: "https://i.ibb.co/9mV52kk9/4058.jpg", admissionNo: "4058", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Ahmed C.M", username: "Ahmed", password: "4055", photo: "https://i.ibb.co/td1c3vV/4053.jpg", admissionNo: "4055", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "ABDUL Basith V.T", username: "Basith", password: "4078", photo: "https://i.ibb.co/gGQL2F3/4078.jpg", admissionNo: "4078", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Hashim E", username: "Hashim", password: "4060", photo: "https://i.ibb.co/y2vMzVb/4060.jpg", admissionNo: "4060", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Hussainsha V.P", username: "Hussainsha", password: "4057", photo: "https://i.ibb.co/JWqLCBx5/4057.jpg", admissionNo: "4057", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Minhal M", username: "Minhal", password: "4064", photo: "https://i.ibb.co/JjH8L3pp/4064.jpg", admissionNo: "4064", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Swalih O", username: "Swalih", password: "4049", photo: "https://i.ibb.co/NdjyWttV/4049.jpg", admissionNo: "4049", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Farhan N.V", username: "Farhan", password: "4062", photo: "https://i.ibb.co/XfS4jw1G/4062.jpg", admissionNo: "4062", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Basith P.P", username: "Basith", password: "4059", photo: "https://i.ibb.co/ZzpzWvsp/4047.jpg", admissionNo: "4059", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Faheem K.T", username: "Faheem", password: "4079", photo: "https://i.ibb.co/TMMgj3Ft/4079.jpg", admissionNo: "4079", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Shanil Muhammed K", username: "Shanil", password: "4041", photo: "https://i.ibb.co/hPZXfpM/4041.jpg", admissionNo: "4041", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Swalih E.P", username: "Swalih", password: "4077", photo: "https://i.ibb.co/HJ1XDHv/4077.jpg", admissionNo: "4066", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Rayyan Ahmed Behishth", username: "Behishth", password: "4043", photo: "https://i.ibb.co/3mRhSJbK/4043.jpg", admissionNo: "4043", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Shab U", username: "Shab", password: "4072", photo: "https://i.ibb.co/Vcx8SWZk/4072.jpg", admissionNo: "4072", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Ahmad Rizan p", username: "Rizan", password: "4066", photo: "https://i.ibb.co/Fkq05QNf/4066.jpg", admissionNo: "4066", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Zahran A.P", username: "Zahran", password: "4045", photo: "https://i.ibb.co/zWkcjkCB/4045.jpg", admissionNo: "4045", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Faheem K.M", username: "faheem", password: "4056", photo: "https://i.ibb.co/f6fvV51/4056.jpg", admissionNo: "4056", studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Rayyan musthafa P.C", username: "Musthafa", password: "4046", photo: "https://i.ibb.co/F4CYqmyf/4046.jpg", admissionNo: "4046", rank: "27" ,studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Hanan C.P", username: "Hanan", password: "4054", photo: "https://via.placeholder.com/100?text=Hanan", admissionNo: "4054", rank: "38" ,studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Muhammed Hadi K", username: "Hadi", password: "4055", photo: "https://i.ibb.co/n80YjVJ4/4055.jpg", admissionNo: "4055", rank: "42" ,studying: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 },
            { name: "Admin", username: "Admin", password: "admin@uswa", photo: "https://i.ibb.co/dyz05HH/image.png", mobileno: "-", teaching: "Darul Huda Islamic University", libraryStatus: "Active", booksIssued: 0, libraryFine: 0 }
        ];      
        
        // Books data array
        let books = [
            {
                id: 1,
                title: "The Holy Quran",
                author: "Allah",
                isbn: "978-9960-50-020-8",
                genre: "Quran",
                status: "available",
                description: "The Holy Quran with translation and commentary",
                cover: "https://i.ibb.co/8X3Q0vF/quran.jpg"
            },
            {
                id: 2,
                title: "Sahih al-Bukhari",
                author: "Imam al-Bukhari",
                isbn: "978-9960-50-021-5",
                genre: "Hadith",
                status: "issued",
                description: "Collection of authentic sayings of Prophet Muhammad (PBUH)",
                cover: "https://i.ibb.co/3RQ7Xt0/bukhari.jpg"
            },
            {
                id: 3,
                title: "Arabic Grammar",
                author: "Dr. V. Abdur Rahim",
                isbn: "978-9960-50-022-2",
                genre: "Arabic Language",
                status: "available",
                description: "Comprehensive guide to Arabic grammar",
                cover: "https://i.ibb.co/0nQqWz0/arabic.jpg"
            },
            {
                id: 4,
                title: "Islamic History",
                author: "Prof. K. Ali",
                isbn: "978-9960-50-023-9",
                genre: "History",
                status: "reserved",
                description: "A detailed history of Islam from its beginning to modern times",
                cover: "https://i.ibb.co/5sRzR9z/history.jpg"
            },
            {
                id: 5,
                title: "Tafsir Ibn Kathir",
                author: "Ibn Kathir",
                isbn: "978-9960-50-024-6",
                genre: "Quran",
                status: "available",
                description: "Classical commentary on the Holy Quran",
                cover: "https://i.ibb.co/0D2vJ0d/tafsir.jpg"
            },
            {
                id: 6,
                title: "Science in Islam",
                author: "Dr. Maurice Bucaille",
                isbn: "978-9960-50-025-3",
                genre: "Science",
                status: "available",
                description: "Exploring scientific facts mentioned in the Quran",
                cover: "https://i.ibb.co/2Z1vJ0d/science.jpg"
            }
        ];
        
        let nextBookId = 7;
        
        // Programs data for each wing
        const wingPrograms = {
            english: [
                {
                    id: 1,
                    name: "Speech Contest",
                    date: "2023-06-01",
                    participation: 14,
                    remarks: "Good",
                    description: "Annual speech competition showcasing public speaking skills",
                    winners: [
                        { rank: 1, name: "Sameeh", wing: "English Wing" },
                        { rank: 2, name: "Rayyan.ek", wing: "English Wing" },
                        { rank: 3, name: "Ameen", wing: "English Wing" }
                    ]
                },
                {
                    id: 2,
                    name: "Spelling Bee",
                    date: "2023-06-10",
                    participation: 23,
                    remarks: "Excellent",
                    description: "Competitive spelling competition testing vocabulary skills",
                    winners: [
                        { rank: 1, name: "Muzammil", wing: "English Wing" },
                        { rank: 2, name: "Zahran", wing: "English Wing" },
                        { rank: 3, name: "Ameen", wing: "English Wing" }
                    ]
                },
                {
                    id: 3,
                    name: "Debate Competition",
                    date: "2023-06-15",
                    participation: 18,
                    remarks: "Very Good",
                    description: "Inter-batch debate competition on current topics",
                    winners: [
                        { rank: 1, name: "Shanil", wing: "English Wing" },
                        { rank: 2, name: "Afnan", wing: "English Wing" },
                        { rank: 3, name: "Masood", wing: "English Wing" }
                    ]
                }
            ],
            arabic: [
                {
                    id: 4,
                    name: "Quran Recitation",
                    date: "2023-05-20",
                    participation: 32,
                    remarks: "Excellent",
                    description: "Holy Quran recitation competition with Tajweed",
                    winners: [
                        { rank: 1, name: "Abdullah.vs", wing: "Arabic Wing" },
                        { rank: 2, name: "Muzammil.na", wing: "Arabic Wing" },
                        { rank: 3, name: "Basith.pp", wing: "Arabic Wing" }
                    ]
                },
                {
                    id: 5,
                    name: "Arabic Speech",
                    date: "2023-06-05",
                    participation: 28,
                    remarks: "Very Good",
                    description: "Arabic language speech competition",
                    winners: [
                        { rank: 1, name: "Ahmed.cm", wing: "Arabic Wing" },
                        { rank: 2, name: "Swalih.o", wing: "Arabic Wing" },
                        { rank: 3, name: "Shanil.k", wing: "Arabic Wing" }
                    ]
                },
                {
                    id: 6,
                    name: "Calligraphy",
                    date: "2023-06-18",
                    participation: 25,
                    remarks: "Good",
                    description: "Islamic calligraphy art competition",
                    winners: [
                        { rank: 1, name: "Farhan", wing: "Arabic Wing" },
                        { rank: 2, name: "Radeef", wing: "Arabic Wing" },
                        { rank: 3, name: "Zahran.ap", wing: "Arabic Wing" }
                    ]
                }
            ],
            acadamic: [
                {
                    id: 7,
                    name: "Science Quiz",
                    date: "2023-05-25",
                    participation: 20,
                    remarks: "Excellent",
                    description: "Inter-batch science quiz competition",
                    winners: [
                        { rank: 1, name: "Shanil", wing: "Academic Wing" },
                        { rank: 2, name: "Afnan", wing: "Academic Wing" },
                        { rank: 3, name: "Masood", wing: "Academic Wing" }
                    ]
                },
                {
                    id: 8,
                    name: "Math Olympiad",
                    date: "2023-06-12",
                    participation: 15,
                    remarks: "Very Good",
                    description: "Mathematics problem-solving competition",
                    winners: [
                        { rank: 1, name: "Zayan", wing: "Academic Wing" },
                        { rank: 2, name: "Rayyan.pk", wing: "Academic Wing" },
                        { rank: 3, name: "Ajuvad ameen.p", wing: "Academic Wing" }
                    ]
                }
            ],
            urdu: [
                {
                    id: 9,
                    name: "Urdu Poetry",
                    date: "2023-05-30",
                    participation: 18,
                    remarks: "Good",
                    description: "Urdu poetry recitation competition",
                    winners: [
                        { rank: 1, name: "Ameen", wing: "Urdu Wing" },
                        { rank: 2, name: "Hanan", wing: "Urdu Wing" },
                        { rank: 3, name: "Hussainsha", wing: "Urdu Wing" }
                    ]
                },
                {
                    id: 10,
                    name: "Urdu Debate",
                    date: "2023-06-20",
                    participation: 16,
                    remarks: "Very Good",
                    description: "Urdu language debate competition",
                    winners: [
                        { rank: 1, name: "Swalih.ep", wing: "Urdu Wing" },
                        { rank: 2, name: "Zayan", wing: "Urdu Wing" },
                        { rank: 3, name: "Hadi.k", wing: "Urdu Wing" }
                    ]
                }
            ],
            malayalam: [
                {
                    id: 11,
                    name: "Malayalam Elocution",
                    date: "2023-06-08",
                    participation: 22,
                    remarks: "Excellent",
                    description: "Malayalam elocution competition",
                    winners: [
                        { rank: 1, name: "Muhammed.mk", wing: "Malayalam Wing" },
                        { rank: 2, name: "Ahmed.cm", wing: "Malayalam Wing" },
                        { rank: 3, name: "Shadhi", wing: "Malayalam Wing" }
                    ]
                },
                {
                    id: 12,
                    name: "Mappila Song",
                    date: "2023-06-22",
                    participation: 20,
                    remarks: "Very Good",
                    description: "Traditional Mappila song competition",
                    winners: [
                        { rank: 1, name: "Faheem.km", wing: "Malayalam Wing" },
                        { rank: 2, name: "Ameensha", wing: "Malayalam Wing" },
                        { rank: 3, name: "Zahran.ap", wing: "Malayalam Wing" }
                    ]
                }
            ],
            library: [
                {
                    id: 13,
                    name: "Book Review",
                    date: "2023-05-15",
                    participation: 12,
                    remarks: "Good",
                    description: "Book review competition",
                    winners: [
                        { rank: 1, name: "Muzammil", wing: "Library Wing" },
                        { rank: 2, name: "Zahran", wing: "Library Wing" },
                        { rank: 3, name: "Ameen", wing: "Library Wing" }
                    ]
                },
                {
                    id: 14,
                    name: "Library Quiz",
                    date: "2023-06-25",
                    participation: 10,
                    remarks: "Excellent",
                    description: "Library and literature quiz competition",
                    winners: [
                        { rank: 1, name: "Shanil", wing: "Library Wing" },
                        { rank: 2, name: "Afnan", wing: "Library Wing" },
                        { rank: 3, name: "Masood", wing: "Library Wing" }
                    ]
                }
            ]
        };
        
        // Current logged-in member and admin
        let currentMember = null;
        let currentAdmin = null;
        let selectedMember = null;
        let selectedAction = '';
        let currentPart = 1; // Track current part being displayed
        let editingBookId = null;
        let currentWing = 'all';
        let currentResultsFilter = 'all';
       
        // Navigation functions
        function showSection(sectionId) {
            document.querySelectorAll('.section').forEach(section => {
                section.classList.remove('active');
            });
            document.getElementById(sectionId).classList.add('active');
           
            // Update active tab
            document.querySelectorAll('nav a').forEach(link => {
                link.classList.remove('active');
            });
            if (event.target.tagName === 'A') {
                event.target.classList.add('active');
            }
           
            // Show logout button if logged in
            updateLogoutButton();
            
            // Initialize library section if it's being shown
            if (sectionId === 'library') {
                populateBooks();
            }
            
            // Initialize reports section if it's being shown
            if (sectionId === 'reports') {
                showAllReports();
            }
        }
       
        // Reports section - show all reports mixed together
        function showAllReports() {
            const reportsContent = document.getElementById('reportsContent');
            
            // Get all programs from all wings
            let programs = [];
            Object.values(wingPrograms).forEach(wingPrograms => {
                programs = programs.concat(wingPrograms);
            });
            
            if (programs.length === 0) {
                reportsContent.innerHTML = `
                    <p style="text-align: center; padding: 30px; color: #004d40; font-size: 1.1rem;">
                        No programs reported yet.
                    </p>
                `;
                return;
            }
            
            let reportsHtml = `
                <table class="report-table">
                    <thead>
                        <tr>
                            <th>Program</th>
                            <th>Date</th>
                            <th>Participation</th>
                            <th>Remarks</th>
                        </tr>
                    </thead>
                    <tbody>
            `;
            
            // Sort programs by date (newest first)
            programs.sort((a, b) => new Date(b.date) - new Date(a.date));
            
            programs.forEach(program => {
                reportsHtml += `
                    <tr>
                        <td>${program.name}</td>
                        <td>${program.date}</td>
                        <td>${program.participation}</td>
                        <td>${program.remarks}</td>
                    </tr>
                `;
            });
            
            reportsHtml += `
                    </tbody>
                </table>
            `;
            
            reportsContent.innerHTML = reportsHtml;
        }
        
        // Show members part
        function showMembersPart(part) {
            currentPart = part;
            
            // Update active button
            document.querySelectorAll('.btn-part').forEach(btn => {
                btn.classList.remove('active');
            });
            event.target.classList.add('active');
            
            // Update part indicator
            document.getElementById('partIndicator').textContent = `Showing Part ${part}`;
            
            // Clear search input
            document.getElementById('memberSearch').value = '';
            
            // Populate members for the selected part
            populateMembersForPart(part);
        }
        
        // Populate members for a specific part
        function populateMembersForPart(part) {
            const membersContainer = document.getElementById('membersContainer');
            membersContainer.innerHTML = '';
            
            // Split members into two parts
            const partSize = Math.ceil(members.length / 2);
            const partMembers = part === 1 ? members.slice(0, partSize) : members.slice(partSize);
            
            partMembers.forEach(member => {
                const memberCard = document.createElement('div');
                memberCard.className = 'member-card';
               
                memberCard.innerHTML = `
                    <img src="${member.photo}" alt="${member.name}" class="member-avatar">
                    <div class="member-name">${member.name}</div>
                    <div class="member-details">Admission No: ${member.admissionNo}</div>
                    <div class="member-details">Library Status: ${member.libraryStatus}</div>
                    <div class="member-details">Books Issued: ${member.booksIssued}</div>
                    <div class="member-details">Fine: ₹${member.libraryFine}</div>
                    <div class="member-actions">
                        <button class="btn-view" onclick="openViewProfileModal('${member.username}')">View Profile</button>
                        ${isAdmin() ? `<button class="btn-fine" onclick="openAddFineModal('${member.username}')">Add Fine</button>` : ''}
                    </div>
                `;
               
                membersContainer.appendChild(memberCard);
            });
        }
       
        // Members section - search functionality
        function filterMembers() {
            const searchTerm = document.getElementById('memberSearch').value.toLowerCase();
            const memberCards = document.querySelectorAll('.member-card');
           
            memberCards.forEach(card => {
                const name = card.querySelector('.member-name').textContent.toLowerCase();
                const admission = card.querySelector('.member-details').textContent.toLowerCase();
               
                if (name.includes(searchTerm) || admission.includes(searchTerm)) {
                    card.style.display = 'block';
                } else {
                    card.style.display = 'none';
                }
            });
        }
       
        // Results section - show results by wing
        function showResults(filter) {
            currentResultsFilter = filter;
            
            // Update active tab
            document.querySelectorAll('.result-tab').forEach(tab => {
                tab.classList.remove('active');
            });
            event.target.classList.add('active');
            
            // Hide all results content
            document.querySelectorAll('.results-content').forEach(content => {
                content.classList.remove('active');
            });
            
            // Show selected results content
            document.getElementById(filter + 'Results').classList.add('active');
            
            // Populate results
            populateResults(filter);
        }
        
        // Populate results for a specific wing or all
        function populateResults(filter) {
            const resultsContainer = document.getElementById(filter + 'Results');
            resultsContainer.innerHTML = '';
            
            let programs = [];
            if (filter === 'all') {
                // Get all programs from all wings
                Object.values(wingPrograms).forEach(wingPrograms => {
                    programs = programs.concat(wingPrograms);
                });
            } else {
                programs = wingPrograms[filter] || [];
            }
            
            if (programs.length === 0) {
                resultsContainer.innerHTML = `
                    <p style="text-align: center; padding: 30px; color: #004d40; font-size: 1.1rem;">
                        No results available for ${filter === 'all' ? 'any wing' : filter + ' wing'} yet.
                    </p>
                `;
                return;
            }
            
            programs.forEach(program => {
                const programCard = document.createElement('div');
                programCard.className = 'program-result-card';
                
                programCard.innerHTML = `
                    <div class="program-result-header">
                        <div class="program-result-title">${program.name}</div>
                        <div class="program-result-date">${program.date}</div>
                    </div>
                    <div class="program-result-info">
                        <div class="program-result-item">
                            <div class="program-result-item-label">Participation</div>
                            <div class="program-result-item-value">${program.participation}</div>
                        </div>
                        <div class="program-result-item">
                            <div class="program-result-item-label">Remarks</div>
                            <div class="program-result-item-value">${program.remarks}</div>
                        </div>
                        <div class="program-result-item">
                            <div class="program-result-item-label">Wing</div>
                            <div class="program-result-item-value">${program.winners[0]?.wing || 'N/A'}</div>
                        </div>
                    </div>
                    <div class="program-winners">
                        <h4><i class="fas fa-trophy"></i> Winners</h4>
                        <div class="winner-grid">
                            ${program.winners.map(winner => `
                                <div class="winner-card">
                                    <div class="winner-medal ${getRankClass(winner.rank)}">
                                        ${getMedalIcon(winner.rank)}
                                    </div>
                                    <div class="winner-card-name">${winner.name}</div>
                                    <div class="winner-card-wing">${winner.wing}</div>
                                </div>
                            `).join('')}
                        </div>
                    </div>
                `;
                
                resultsContainer.appendChild(programCard);
            });
        }
        
        // Helper function to get rank class
        function getRankClass(rank) {
            if (rank === 1) return 'first';
            if (rank === 2) return 'second';
            if (rank === 3) return 'third';
            return '';
        }
        
        // Helper function to get medal icon
        function getMedalIcon(rank) {
            if (rank === 1) return '🥇';
            if (rank === 2) return '🥈';
            if (rank === 3) return '🥉';
            return '';
        }
        
        // Library section - populate books
        function populateBooks() {
            const booksContainer = document.getElementById('booksContainer');
            booksContainer.innerHTML = '';
            
            books.forEach(book => {
                const bookCard = document.createElement('div');
                bookCard.className = 'book-card';
                
                const statusClass = book.status === 'available' ? 'available' : 
                                  book.status === 'issued' ? 'issued' : 'reserved';
                
                bookCard.innerHTML = `
                    <img src="${book.cover}" alt="${book.title}" class="book-cover">
                    <div class="book-title">${book.title}</div>
                    <div class="book-details"><strong>Author:</strong> ${book.author}</div>
                    <div class="book-details"><strong>ISBN:</strong> ${book.isbn}</div>
                    <div class="book-details"><strong>Genre:</strong> ${book.genre}</div>
                    <div class="book-status ${statusClass}">${book.status.charAt(0).toUpperCase() + book.status.slice(1)}</div>
                    <div class="book-actions">
                        ${book.status === 'available' ? 
                            `<button class="btn-issue" onclick="issueBook(${book.id})">Issue</button>` : 
                            book.status === 'issued' ? 
                            `<button class="btn-return" onclick="returnBook(${book.id})">Return</button>` : 
                            `<button class="btn-reserve" onclick="reserveBook(${book.id})">Reserve</button>`
                        }
                        ${isAdmin() ? `
                            <button class="btn-edit" onclick="editBook(${book.id})">Edit</button>
                            <button class="btn-delete" onclick="deleteBook(${book.id})">Delete</button>
                        ` : ''}
                    </div>
                `;
                
                booksContainer.appendChild(bookCard);
            });
        }
        
        // Library section - filter books
        function filterBooks() {
            const searchTerm = document.getElementById('bookSearch').value.toLowerCase();
            const bookCards = document.querySelectorAll('.book-card');
            
            bookCards.forEach(card => {
                const title = card.querySelector('.book-title').textContent.toLowerCase();
                const details = card.querySelectorAll('.book-details');
                
                let match = title.includes(searchTerm);
                details.forEach(detail => {
                    if (detail.textContent.toLowerCase().includes(searchTerm)) {
                        match = true;
                    }
                });
                
                card.style.display = match ? 'block' : 'none';
            });
        }
        
        // Library section - add book
        function openAddBookModal() {
            // Only allow admin to add books
            if (!isAdmin()) {
                alert('Only admin can add books. Please login as admin.');
                showSection('adminLogin');
                return;
            }
            
            document.getElementById('addBookForm').reset();
            document.getElementById('addBookModal').style.display = 'flex';
        }
        
        function closeAddBookModal() {
            document.getElementById('addBookModal').style.display = 'none';
        }
        
        function addBook() {
            if (!isAdmin()) {
                alert('Only admin can add books');
                return;
            }
            
            const title = document.getElementById('bookTitle').value;
            const author = document.getElementById('bookAuthor').value;
            const isbn = document.getElementById('bookISBN').value;
            const genre = document.getElementById('bookGenre').value;
            const status = document.getElementById('bookStatus').value;
            const description = document.getElementById('bookDescription').value;
            
            if (!title || !author || !isbn || !genre || !status) {
                alert('Please fill in all required fields');
                return;
            }
            
            // Check if ISBN already exists
            if (books.some(book => book.isbn === isbn)) {
                alert('A book with this ISBN already exists');
                return;
            }
            
            // Add the new book
            const newBook = {
                id: nextBookId++,
                title,
                author,
                isbn,
                genre,
                status,
                description,
                cover: `https://i.ibb.co/${Math.random().toString(36).substring(7)}/book.jpg`
            };
            
            books.push(newBook);
            closeAddBookModal();
            populateBooks();
            
            alert('Book added successfully!');
        }
        
        // Library section - edit book
        function editBook(bookId) {
            if (!isAdmin()) {
                alert('Only admin can edit books');
                return;
            }
            
            const book = books.find(b => b.id === bookId);
            if (!book) return;
            
            editingBookId = bookId;
            
            // Populate the edit form
            document.getElementById('editBookTitle').value = book.title;
            document.getElementById('editBookAuthor').value = book.author;
            document.getElementById('editBookISBN').value = book.isbn;
            document.getElementById('editBookGenre').value = book.genre;
            document.getElementById('editBookStatus').value = book.status;
            document.getElementById('editBookDescription').value = book.description || '';
            
            document.getElementById('editBookModal').style.display = 'flex';
        }
        
        function closeEditBookModal() {
            document.getElementById('editBookModal').style.display = 'none';
            editingBookId = null;
        }
        
        function updateBook() {
            if (!isAdmin()) {
                alert('Only admin can update books');
                return;
            }
            
            const title = document.getElementById('editBookTitle').value;
            const author = document.getElementById('editBookAuthor').value;
            const isbn = document.getElementById('editBookISBN').value;
            const genre = document.getElementById('editBookGenre').value;
            const status = document.getElementById('editBookStatus').value;
            const description = document.getElementById('editBookDescription').value;
            
            if (!title || !author || !isbn || !genre || !status) {
                alert('Please fill in all required fields');
                return;
            }
            
            // Check if ISBN already exists (excluding current book)
            if (books.some(book => book.isbn === isbn && book.id !== editingBookId)) {
                alert('A book with this ISBN already exists');
                return;
            }
            
            // Update the book
            const bookIndex = books.findIndex(b => b.id === editingBookId);
            if (bookIndex !== -1) {
                books[bookIndex] = {
                    ...books[bookIndex],
                    title,
                    author,
                    isbn,
                    genre,
                    status,
                    description
                };
                
                closeEditBookModal();
                populateBooks();
                
                alert('Book updated successfully!');
            }
        }
        
        // Library section - delete book
        function deleteBook(bookId) {
            if (!isAdmin()) {
                alert('Only admin can delete books');
                return;
            }
            
            if (confirm('Are you sure you want to delete this book?')) {
                books = books.filter(book => book.id !== bookId);
                populateBooks();
                alert('Book deleted successfully!');
            }
        }
        
        // Library section - issue book
        function issueBook(bookId) {
            if (!currentMember) {
                alert('Please login to issue a book');
                showSection('login');
                return;
            }
            
            const book = books.find(b => b.id === bookId);
            if (!book) return;
            
            if (book.status !== 'available') {
                alert('This book is not available for issue');
                return;
            }
            
            // Check if member has reached book limit
            if (currentMember.booksIssued >= 3) {
                alert('You have reached the maximum limit of issued books (3)');
                return;
            }
            
            // Issue the book
            book.status = 'issued';
            currentMember.booksIssued += 1;
            
            // Update the profile if viewing it
            if (document.getElementById('profile').classList.contains('active')) {
                populateProfile(currentMember);
            }
            
            populateBooks();
            alert('Book issued successfully!');
        }
        
        // Library section - return book
        function returnBook(bookId) {
            if (!currentMember) {
                alert('Please login to return a book');
                showSection('login');
                return;
            }
            
            const book = books.find(b => b.id === bookId);
            if (!book) return;
            
            if (book.status !== 'issued') {
                alert('This book is not currently issued');
                return;
            }
            
            // Return the book
            book.status = 'available';
            currentMember.booksIssued -= 1;
            
            // Update the profile if viewing it
            if (document.getElementById('profile').classList.contains('active')) {
                populateProfile(currentMember);
            }
            
            populateBooks();
            alert('Book returned successfully!');
        }
        
        // Library section - reserve book
        function reserveBook(bookId) {
            if (!currentMember) {
                alert('Please login to reserve a book');
                showSection('login');
                return;
            }
            
            const book = books.find(b => b.id === bookId);
            if (!book) return;
            
            if (book.status !== 'available') {
                alert('This book is not available for reservation');
                return;
            }
            
            // Reserve the book
            book.status = 'reserved';
            populateBooks();
            alert('Book reserved successfully!');
        }
       
        // Login functionality with members data
        function attemptLogin() {
            const username = document.getElementById('username').value;
            const password = document.getElementById('password').value;
           
            // Find member with matching credentials
            const member = members.find(m => m.username === username && m.password === password);
           
            if (member) {
                currentMember = member;
                showSection('profile');
                updateLogoutButton();
                populateProfile(member);
                alert(`Login successful! Welcome ${member.name}!`);
            } else {
                alert('Invalid username or password. Please try again.');
            }
        }
       
        // Admin Login functionality
        function attemptAdminLogin() {
            const username = document.getElementById('adminUsername').value;
            const password = document.getElementById('adminPassword').value;
           
            // Find admin with matching credentials
            const admin = members.find(m => m.username === username && m.password === password);
           
            if (admin) {
                currentAdmin = admin;
                showSection('adminHome');
                updateLogoutButton();
                alert(`Admin login successful! Welcome ${admin.name}!`);
            } else {
                alert('Invalid admin username or password. Please try again.');
            }
        }
       
        // Update logout button visibility
        function updateLogoutButton() {
            const logoutBtn = document.getElementById('logoutBtn');
            if (currentMember || currentAdmin) {
                logoutBtn.style.display = 'block';
            } else {
                logoutBtn.style.display = 'none';
            }
        }
       
        // Logout functionality
        function logout() {
            currentMember = null;
            currentAdmin = null;
            selectedMember = null;
            updateLogoutButton();
            alert('You have been logged out successfully!');
        }
       
        // Check if user is admin
        function isAdmin() {
            return currentAdmin && currentAdmin.username === 'Admin';
        }
       
        // Open Add Fine Modal
        function openAddFineModal(username) {
            // Only allow admin to add fines
            if (!isAdmin()) {
                alert('Only admin can add fines. Please login as admin.');
                showSection('adminLogin');
                return;
            }
            
            // Find the member
            const member = members.find(m => m.username === username);
            if (member) {
                selectedMember = member;
            }
           
            // Reset form
            document.getElementById('addFineForm').reset();
           
            // Show the modal
            document.getElementById('addFineModal').style.display = 'flex';
        }
       
        // Add Fine functionality
        function addFine() {
            if (!isAdmin()) {
                alert('Only admin can add fines');
                return;
            }
            
            if (!selectedMember) {
                alert('No member selected');
                return;
            }
           
            const fineAmount = parseInt(document.getElementById('addFineAmount').value);
            const fineReason = document.getElementById('addFineReason').value;
           
            if (!fineAmount || !fineReason) {
                alert('Please fill in all required fields');
                return;
            }
           
            // Add the fine to the member
            selectedMember.libraryFine += fineAmount;
            closeAddFineModal();
           
            // If viewing profile, update it
            if (currentMember && currentMember.username === selectedMember.username) {
                populateProfile(selectedMember);
            }
            
            // Refresh the current members part
            populateMembersForPart(currentPart);
           
            alert(`Fine of ₹${fineAmount} added successfully! Reason: ${fineReason}`);
        }
       
        // Close Add Fine Modal
        function closeAddFineModal() {
            document.getElementById('addFineModal').style.display = 'none';
        }
       
        // Open Remove Fine Modal
        function openRemoveFineModal() {
            // Only allow admin to remove fines
            if (!isAdmin()) {
                alert('Only admin can remove fines. Please login as admin.');
                showSection('adminLogin');
                return;
            }
           
            // Reset form
            document.getElementById('removeFineForm').reset();
           
            // Show the modal
            document.getElementById('removeFineModal').style.display = 'flex';
        }
       
        // Remove Fine functionality
        function removeFine() {
            if (!isAdmin()) {
                alert('Only admin can remove fines');
                return;
            }
            
            if (!currentMember) {
                alert('No member selected');
                return;
            }
           
            const removeAmount = parseInt(document.getElementById('removeFineAmount').value);
            const removeReason = document.getElementById('removeReason').value;
           
            if (!removeAmount || !removeReason) {
                alert('Please fill in all required fields');
                return;
            }
           
            // Ensure we don't remove more than the current fine amount
            const actualRemoveAmount = Math.min(removeAmount, currentMember.libraryFine);
            currentMember.libraryFine -= actualRemoveAmount;
           
            closeRemoveFineModal();
           
            // Update the profile
            populateProfile(currentMember);
            
            // Refresh the current members part
            populateMembersForPart(currentPart);
           
            if (actualRemoveAmount < removeAmount) {
                alert(`Removed ₹${actualRemoveAmount} (could not remove more than current fine of ₹${currentMember.libraryFine + actualRemoveAmount})`);
            } else {
                alert(`Fine of ₹${actualRemoveAmount} removed successfully! Reason: ${removeReason}`);
            }
        }
       
        // Close Remove Fine Modal
        function closeRemoveFineModal() {
            document.getElementById('removeFineModal').style.display = 'none';
        }
       
        // Open View Profile Modal
        function openViewProfileModal(username) {
            // Store the username in the modal for later use
            document.getElementById('profileUsername').value = username;
            document.getElementById('profilePassword').value = '';
           
            // Show the modal
            document.getElementById('viewProfileModal').style.display = 'flex';
        }
       
        // Close View Profile Modal
        function closeViewProfileModal() {
            document.getElementById('viewProfileModal').style.display = 'none';
        }
       
        // View Profile functionality
        function viewProfile() {
            const username = document.getElementById('profileUsername').value;
            const password = document.getElementById('profilePassword').value;
           
            // Find member with matching credentials
            const member = members.find(m => m.username === username && m.password === password);
           
            if (member) {
                currentMember = member;
                closeViewProfileModal();
                showSection('profile');
                populateProfile(member);
            } else {
                alert('Invalid username or password. Please try again.');
            }
        }
       
        // Populate Profile page with member data
        function populateProfile(member) {
            document.getElementById('profileAvatar').src = member.photo;
            document.getElementById('profileName').textContent = member.name;
            document.getElementById('profileAdmissionNo').textContent = `Admission No: ${member.admissionNo}`;
            document.getElementById('profileMobile').textContent = member.mobile || 'Not Available';
            document.getElementById('profileDob').textContent = member.dateOfBirth || 'Not Available';
            document.getElementById('profileRank').textContent = member.rank || 'Not Available';
            document.getElementById('profileStudying').textContent = member.studying || 'Not Available';
            document.getElementById('profileLibraryStatus').textContent = member.libraryStatus || 'Not Available';
            document.getElementById('profileBooksIssued').textContent = member.booksIssued || 'Not Available';
            document.getElementById('profileLibraryFine').textContent = `₹${member.libraryFine || 0}`;
            
            // Update fine status card
            updateFineStatusCard(member);
            
            // Show/hide admin buttons based on user role
            const addFineBtn = document.getElementById('addFineBtn');
            const removeFineBtn = document.getElementById('removeFineBtn');
            
            if (isAdmin()) {
                addFineBtn.style.display = 'inline-block';
                removeFineBtn.style.display = 'inline-block';
            } else {
                addFineBtn.style.display = 'none';
                removeFineBtn.style.display = 'none';
            }
        }
        
        // Update fine status card
        function updateFineStatusCard(member) {
            const fineAmount = member.libraryFine || 0;
            const fineAmountElement = document.getElementById('profileFineAmount');
            const fineMessageElement = document.getElementById('profileFineMessage');
            
            fineAmountElement.textContent = `₹${fineAmount}`;
            
            if (fineAmount > 0) {
                fineMessageElement.textContent = 'Pending fines - Please pay at the admin office';
                fineAmountElement.style.color = '#e74c3c';
            } else {
                fineMessageElement.textContent = 'No pending fines';
                fineAmountElement.style.color = '#4caf50';
            }
        }
       
        // Open Cash Modal
        function openCashModal() {
            if (!currentMember) {
                alert('No member selected');
                return;
            }
            
            // Only allow admin to process cash payments
            if (!isAdmin()) {
                alert('Only admin can process cash payments');
                return;
            }
            
            // Set the cash section with the current member's details
            document.getElementById('cashName').textContent = currentMember.name;
            document.getElementById('cashAdmissionNo').textContent = currentMember.admissionNo;
            document.getElementById('cashAmount').textContent = `₹${currentMember.libraryFine}`;
            
            // Show the cash section
            showSection('cash');
        }
        
        // Process Cash Payment
        function processCashPayment() {
            if (!isAdmin()) {
                alert('Only admin can process cash payments');
                return;
            }
            
            if (!currentMember) {
                alert('No member selected');
                return;
            }
            
            // Process the payment
            const paymentAmount = currentMember.libraryFine;
            currentMember.libraryFine = 0;
            
            // Update the profile
            populateProfile(currentMember);
            
            // Refresh the current members part
            populateMembersForPart(currentPart);
            
            alert(`Payment of ₹${paymentAmount} processed successfully!`);
            
            // Go back to the profile
            showSection('profile');
        }
       
        // Pay Fine functionality
        function payFine() {
            if (!isAdmin()) {
                alert('Please login as admin to process fine payments');
                showSection('adminLogin');
                return;
            }
           
            const fineStatus = document.getElementById('fineStatus');
            fineStatus.textContent = 'Paid';
            fineStatus.style.color = '#4caf50';
           
            // Update member's fine amount
            const username = document.getElementById('fineName').textContent;
            const member = members.find(m => m.name === username);
            
            if (member) {
                member.libraryFine = 0;
                populateProfile(member);
                populateMembersForPart(currentPart);
            }
           
            alert('Fine paid successfully!');
        }
        
        // Add Report Modal Functions
        function openAddReportModal() {
            document.getElementById('addReportModal').style.display = 'flex';
        }
        
        function closeAddReportModal() {
            document.getElementById('addReportModal').style.display = 'none';
        }
        
        function addReport() {
            const programName = document.getElementById('programName').value;
            const programDate = document.getElementById('programDate').value;
            const participation = document.getElementById('participation').value;
            const remarks = document.getElementById('remarks').value;
            
            if (!programName || !programDate || !participation || !remarks) {
                alert('Please fill in all fields');
                return;
            }
            
            // Create new program object
            const newProgram = {
                id: Date.now(), // Simple ID generation
                name: programName,
                date: programDate,
                participation: parseInt(participation),
                remarks: remarks,
                description: "Newly added program",
                winners: [
                    { rank: 1, name: "TBD", wing: "General" },
                    { rank: 2, name: "TBD", wing: "General" },
                    { rank: 3, name: "TBD", wing: "General" }
                ]
            };
            
            // Add to a default wing, say 'general'
            if (!wingPrograms['general']) {
                wingPrograms['general'] = [];
            }
            wingPrograms['general'].push(newProgram);
            
            closeAddReportModal();
            
            // Refresh the reports display
            showAllReports();
            
            // Refresh results if needed
            if (currentResultsFilter === 'all' || currentResultsFilter === 'general') {
                populateResults(currentResultsFilter);
            }
            
            alert('Report added successfully!');
        }
       
        // Open Members Selection Modal
        function openMembersSelectionModal(action) {
            selectedAction = action;
            document.getElementById('membersSearchInput').value = '';
            populateMembersSelectionGrid();
            document.getElementById('membersSelectionModal').style.display = 'flex';
        }
       
        // Close Members Selection Modal
        function closeMembersSelectionModal() {
            document.getElementById('membersSelectionModal').style.display = 'none';
        }
       
        // Populate Members Selection Grid
        function populateMembersSelectionGrid() {
            const grid = document.getElementById('membersSelectionGrid');
            grid.innerHTML = '';
           
            members.forEach(member => {
                const card = document.createElement('div');
                card.className = 'member-selection-card';
                
                card.innerHTML = `
                    <img src="${member.photo}" alt="${member.name}" class="member-selection-avatar">
                    <div class="member-selection-name">${member.name}</div>
                    <div class="member-selection-admission">Admission: ${member.admissionNo}</div>
                    <div class="member-selection-actions">
                        <button onclick="selectMember('${member.username}')">Select</button>
                    </div>
                `;
               
                grid.appendChild(card);
            });
        }
       
        // Search in Members Selection Modal
        function searchMembersSelection() {
            const searchTerm = document.getElementById('membersSearchInput').value.toLowerCase();
            const cards = document.querySelectorAll('.member-selection-card');
           
            cards.forEach(card => {
                const name = card.querySelector('.member-selection-name').textContent.toLowerCase();
                const admission = card.querySelector('.member-selection-admission').textContent.toLowerCase();
               
                if (name.includes(searchTerm) || admission.includes(searchTerm)) {
                    card.style.display = 'block';
                } else {
                    card.style.display = 'none';
                }
            });
        }
       
        // Select a member in the Members Selection Modal
        function selectMember(username) {
            // Remove selection from all cards
            document.querySelectorAll('.member-selection-card').forEach(card => {
                card.classList.remove('selected');
            });
           
            // Add selection to the clicked card
            event.target.closest('.member-selection-card').classList.add('selected');
           
            // Store the selected member
            selectedMember = members.find(m => m.username === username);
        }
       
        // Confirm member selection
        function confirmMemberSelection() {
            if (!selectedMember) {
                alert('Please select a member first');
                return;
            }
           
            if (selectedAction === 'addFine') {
                // Open the add fine modal with the selected member
                openAddFineModal(selectedMember.username);
                closeMembersSelectionModal();
            } else if (selectedAction === 'processCash') {
                // Set the selected member as current member and open cash section
                currentMember = selectedMember;
                closeMembersSelectionModal();
                openCashModal();
            }
        }
        
        // Initialize the page
        document.addEventListener('DOMContentLoaded', function() {
            // Show Part 1 by default
            populateMembersForPart(1);
            
            // Initialize results with all programs
            populateResults('all');
            
            // Initialize reports with all programs
            showAllReports();
        });
       
        // Close modal when clicking outside
        window.onclick = function(event) {
            const modals = document.querySelectorAll('.modal');
            modals.forEach(modal => {
                if (event.target === modal) {
                    modal.style.display = 'none';
                }
            });
        }
    </script>
</body>
</html>
