
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Project Team Dashboard</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    }
    
    body {
      background: linear-gradient(135deg, #f8fafc 0%, #e2e8f0 100%);
      min-height: 100vh;
      padding: 20px;
    }
    
    .header {
      background: linear-gradient(90deg, #1e293b 0%, #0f172a 100%);
      color: white;
      padding: 32px;
      border-radius: 12px;
      margin-bottom: 24px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    }
    
    .header h1 {
      font-size: 28px;
      font-weight: 700;
      margin-bottom: 8px;
      display: flex;
      align-items: center;
      gap: 12px;
    }
    
    .header p {
      color: #cbd5e1;
      font-size: 16px;
    }
    
    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
      margin-bottom: 32px;
    }
    
    .stat-card {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      display: flex;
      align-items: center;
      gap: 16px;
    }
    
    .stat-icon {
      width: 40px;
      height: 40px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: bold;
      color: white;
      font-size: 18px;
    }
    
    .blue { background: #3b82f6; }
    .green { background: #10b981; }
    .orange { background: #f97316; }
    .purple { background: #8b5cf6; }
    
    .stat-info h3 {
      font-size: 14px;
      color: #64748b;
      margin-bottom: 4px;
    }
    
    .stat-info p {
      font-size: 20px;
      font-weight: 700;
      color: #1e293b;
    }
    
    .team-member {
      background: white;
      border-radius: 12px;
      overflow: hidden;
      margin-bottom: 16px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      transition: all 0.2s ease;
    }
    
    .team-member:hover {
      box-shadow: 0 4px 8px rgba(0,0,0,0.15);
    }
    
    .team-member.jayanna {
      border: 2px
    }
    
    .member-header {
      padding: 24px;
      cursor: pointer;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    
    .member-info {
      display: flex;
      gap: 16px;
      flex: 1;
    }
    
    .avatar {
      width: 48px;
      height: 48px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: bold;
      color: white;
      font-size: 18px;
    }
    
    .member-details {
      flex: 1;
      min-width: 0;
    }
    
    .member-details h2 {
      font-size: 20px;
      font-weight: 700;
      color: #1e293b;
      margin-bottom: 4px;
      overflow: hidden;
      text-overflow: ellipsis;
    }
    
    .member-details .usi {
      font-size: 14px;
      color: #64748b;
      margin-bottom: 4px;
    }
    
    .member-details .role {
      font-size: 16px;
      color: #475569;
      font-weight: 600;
    }
    
    .expand-btn {
      background: none;
      border: none;
      font-size: 20px;
      color: #94a3b8;
      cursor: pointer;
      width: 32px;
      height: 32px;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    
    .tasks-section {
      padding: 0 24px 24px 24px;
      border-top: 1px solid #e2e8f0;
    }
    
    .tasks-section h3 {
      font-size: 16px;
      font-weight: 600;
      color: #475569;
      margin: 16px 0 12px 0;
      display: flex;
      align-items: center;
      gap: 8px;
    }
    
    .task-item {
      display: flex;
      gap: 12px;
      padding: 12px;
      background: #f8fafc;
      border-radius: 8px;
      margin-bottom: 8px;
    }
    
    .task-number {
      width: 24px;
      height: 24px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 12px;
      font-weight: bold;
      color: white;
      flex-shrink: 0;
    }
    
    .task-text {
      flex: 1;
      font-size: 14px;
      color: #475569;
      line-height: 1.5;
    }
    
    @media (max-width: 768px) {
      .header {
        padding: 24px;
      }
      
      .header h1 {
        font-size: 24px;
      }
      
      .stats-grid {
        grid-template-columns: 1fr;
      }
      
      .member-header {
        flex-direction: column;
        gap: 16px;
        text-align: center;
      }
    }
  </style>
</head>
<body>
  <div class="header">
    <h1>👥 Project Team Dashboard</h1>
    <p>Waterfall Model Development Team</p>
  </div>

  <div class="stats-grid">
    <div class="stat-card">
      <div class="stat-icon blue">👥</div>
      <div class="stat-info">
        <h3>Team Members</h3>
        <p>5</p>
      </div>
    </div>
    <div class="stat-card">
      <div class="stat-icon purple">📋</div>
      <div class="stat-info">
        <h3>Total Tasks</h3>
        <p>13</p>
      </div>
    </div>
  </div>

  <div class="team-member jayanna">
    <div class="member-header">
      <div class="member-info">
        <div class="avatar" style="background: #ec4899;">JG</div>
        <div class="member-details">
          <h2>Jayanna Gibson</h2>
          <div class="usi">USI: 1054094</div>
          <div class="role">UI/UX Designer & Front-End Developer</div>
        </div>
      </div>
      <button class="expand-btn">▼</button>
    </div>
    <div class="tasks-section" style="display: none;">
      <h3>📋 Assigned Tasks</h3>
      <div class="task-item">
        <div class="task-number" style="background: #ec4899;">1</div>
        <div class="task-text">Contribute to Work Breakdown and Timeline: outline user-interface design phase, front-end milestones.</div>
      </div>
      <div class="task-item">
        <div class="task-number" style="background: #ec4899;">2</div>
        <div class="task-text">Assist Project Manager in creating Gantt Chart (showing design → development → testing).</div>
      </div>
    </div>
  </div>

  <div class="team-member">
    <div class="member-header">
      <div class="member-info">
        <div class="avatar" style="background: #3b82f6;">SM</div>
        <div class="member-details">
          <h2>Shashwat Mishra</h2>
          <div class="usi">USI: 1052319</div>
          <div class="role">Project Manager & System Architect</div>
        </div>
      </div>
      <button class="expand-btn">▼</button>
    </div>
    <div class="tasks-section" style="display: none;">
      <h3>📋 Assigned Tasks</h3>
      <div class="task-item">
        <div class="task-number" style="background: #3b82f6;">1</div>
        <div class="task-text">Write the Introduction section (define the project problem, goals, scope, constraints).</div>
      </div>
      <div class="task-item">
        <div class="task-number" style="background: #3b82f6;">2</div>
        <div class="task-text">Approve all other sections and compile final PDF.</div>
      </div>
      <div class="task-item">
        <div class="task-number" style="background: #3b82f6;">3</div>
        <div class="task-text">Ensure timeline and deliverables align with the Waterfall model stages.</div>
      </div>
      <div class="task-item">
        <div class="task-number" style="background: #3b82f6;">4</div>
        <div class="task-text">Draft Hardware and Software Requirements section.</div>
      </div>
    </div>
  </div>

  <div class="team-member">
    <div class="member-header">
      <div class="member-info">
        <div class="avatar" style="background: #8b5cf6;">SP</div>
        <div class="member-details">
          <h2>Suchitra Patil</h2>
          <div class="usi">USI: 1046144</div>
          <div class="role">Lead Software Engineer (Backend & Integration)</div>
        </div>
      </div>
      <button class="expand-btn">▼</button>
    </div>
    <div class="tasks-section" style="display: none;">
      <h3>📋 Assigned Tasks</h3>
      <div class="task-item">
        <div class="task-number" style="background: #8b5cf6;">1</div>
        <div class="task-text">Specify backend stack (server, DBMS, frameworks) and integration needs.</div>
      </div>
      <div class="task-item">
        <div class="task-number" style="background: #8b5cf6;">2</div>
        <div class="task-text">Provide technical input for Work Breakdown Structure (WBS).</div>
      </div>
    </div>
  </div>

  <div class="team-member">
    <div class="member-header">
      <div class="member-info">
        <div class="avatar" style="background: #f97316;">KS</div>
        <div class="member-details">
          <h2>Kalief Sobers</h2>
          <div class="usi">USI: 1047966</div>
          <div class="role">Quality Assurance & Risk Manager</div>
        </div>
      </div>
      <button class="expand-btn">▼</button>
    </div>
    <div class="tasks-section" style="display: none;">
      <h3>📋 Assigned Tasks</h3>
      <div class="task-item">
        <div class="task-number" style="background: #f97316;">1</div>
        <div class="task-text">Write the Risk Analysis section (identify ≥ 5 specific risks such as data-loss, offline-sync failure, resource shortage, etc.).</div>
      </div>
      <div class="task-item">
        <div class="task-number" style="background: #f97316;">2</div>
        <div class="task-text">Define mitigation and monitoring strategies.</div>
      </div>
      <div class="task-item">
        <div class="task-number" style="background: #f97316;">3</div>
        <div class="task-text">Support test-phase planning in the schedule.</div>
      </div>
    </div>
  </div>

  <div class="team-member">
    <div class="member-header">
      <div class="member-info">
        <div class="avatar" style="background: #10b981;">KI</div>
        <div class="member-details">
          <h2>Kiesheena Inniss</h2>
          <div class="usi">USI: 1051541</div>
          <div class="role">Business Analyst & Documentation Specialist</div>
        </div>
      </div>
      <button class="expand-btn">▼</button>
    </div>
    <div class="tasks-section" style="display: none;">
      <h3>📋 Assigned Tasks</h3>
      <div class="task-item">
        <div class="task-number" style="background: #10b981;">1</div>
        <div class="task-text">Write the Project Organisation section (describe team hierarchy, communication, responsibilities).</div>
      </div>
      <div class="task-item">
        <div class="task-number" style="background: #10b981;">2</div>
        <div class="task-text">Prepare the Group Summary Page (division of labour, collaboration methods, challenges).</div>
      </div>
    </div>
  </div>

  <script>
    // Simple expand/collapse functionality
    document.querySelectorAll('.expand-btn').forEach((button, index) => {
      button.addEventListener('click', () => {
        const tasksSection = button.closest('.team-member').querySelector('.tasks-section');
        const isExpanded = tasksSection.style.display === 'block';
        
        if (isExpanded) {
          tasksSection.style.display = 'none';
          button.textContent = '▼';
        } else {
          tasksSection.style.display = 'block';
          button.textContent = '▲';
        }
      });
    });
  </script>
</body>
</html>
