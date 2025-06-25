---
permalink: /courses/
title: "Course Progress"
layout: single
toc: true
toc_sticky: true
---

<style>
.course-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  margin: 20px 0;
}

.course-card {
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  border: 2px solid #00ff41;
  border-radius: 15px;
  padding: 20px;
  text-align: center;
  transition: all 0.3s ease;
  cursor: pointer;
  position: relative;
  overflow: hidden;
}

.course-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 35px rgba(0, 255, 65, 0.3);
  border-color: #00ff88;
}

.course-icon {
  width: 80px;
  height: 80px;
  margin: 0 auto 15px;
  border-radius: 50%;
  background: linear-gradient(45deg, #00ff41, #00cc33);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2.5em;
  color: #000;
}

.course-code {
  color: #00ff41;
  font-family: 'Courier New', monospace;
  font-weight: bold;
  font-size: 1.1em;
  margin: 10px 0 5px;
}

.course-title {
  color: #ffffff;
  font-size: 1em;
  margin: 5px 0 10px;
  line-height: 1.3;
}

.course-status {
  display: inline-block;
  padding: 5px 15px;
  border-radius: 20px;
  font-size: 0.8em;
  font-weight: bold;
  margin: 10px 0;
  background: rgba(128, 128, 128, 0.3);
  color: #cccccc;
}

.phase-header {
  background: linear-gradient(135deg, #2E5090, #4A69BD);
  color: white;
  padding: 20px;
  margin: 30px 0 20px 0;
  border-radius: 10px;
  text-align: center;
  font-size: 1.5em;
  font-weight: bold;
}

.progress-overview {
  background: rgba(0, 255, 65, 0.1);
  border: 2px solid #00ff41;
  border-radius: 15px;
  padding: 25px;
  margin: 20px 0;
  text-align: center;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 20px;
  margin: 20px 0;
}

.stat-card {
  background: rgba(0, 255, 65, 0.1);
  border: 1px solid #00ff41;
  border-radius: 10px;
  padding: 20px;
  text-align: center;
}

.stat-number {
  font-size: 2.5em;
  font-weight: bold;
  color: #00ff41;
  display: block;
}

.stat-label {
  color: #cccccc;
  font-size: 0.9em;
  margin-top: 5px;
}

.modal {
  display: none;
  position: fixed;
  z-index: 1000;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);
}

.modal-content {
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  margin: 5% auto;
  padding: 30px;
  border: 2px solid #00ff41;
  border-radius: 15px;
  width: 90%;
  max-width: 800px;
  max-height: 80vh;
  overflow-y: auto;
  color: #ffffff;
}

.close {
  color: #00ff41;
  float: right;
  font-size: 28px;
  font-weight: bold;
  cursor: pointer;
}

.notes-area {
  width: 100%;
  min-height: 200px;
  background: #0d1117;
  border: 1px solid #00ff41;
  border-radius: 8px;
  padding: 15px;
  color: #ffffff;
  font-family: 'Courier New', monospace;
  resize: vertical;
  margin: 15px 0;
}

.save-btn {
  background: linear-gradient(45deg, #00ff41, #00cc33);
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  color: #000;
  font-weight: bold;
  cursor: pointer;
  margin: 10px 5px;
}

@media (max-width: 768px) {
  .course-grid { grid-template-columns: 1fr; }
  .stats-grid { grid-template-columns: repeat(2, 1fr); }
}
</style>

# 🎯 Course Progress Overview

<div class="progress-overview">
  <h2>📊 Overall Progress</h2>
  <div class="stats-grid">
    <div class="stat-card">
      <span class="stat-number">0</span>
      <span class="stat-label">Courses Started</span>
    </div>
    <div class="stat-card">
      <span class="stat-number">0</span>
      <span class="stat-label">Courses Completed</span>
    </div>
    <div class="stat-card">
      <span class="stat-number">19</span>
      <span class="stat-label">Total Courses</span>
    </div>
    <div class="stat-card">
      <span class="stat-number">60</span>
      <span class="stat-label">Months Remaining</span>
    </div>
  </div>
</div>

---

<div class="phase-header">
📚 BACHELOR'S PHASE (Months 1-24)
</div>

## Foundation Block (Months 1-12)

<div class="course-grid">
  <div class="course-card" onclick="openCourseModal('bacs3275')">
    <div class="course-icon">🖥️</div>
    <div class="course-code">BACS 3275</div>
    <div class="course-title">Foundations: Computers, Technology & Security</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('bacs3301')">
    <div class="course-icon">🛡️</div>
    <div class="course-code">BACS 3301</div>
    <div class="course-title">Introduction to Cybersecurity</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('bacs3402')">
    <div class="course-icon">✍️</div>
    <div class="course-code">BACS 3402</div>
    <div class="course-title">Effective Cyber Writing and Speaking</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('bacs3401')">
    <div class="course-icon">🔐</div>
    <div class="course-code">BACS 3401</div>
    <div class="course-title">Security Essentials</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('bacs3504')">
    <div class="course-icon">🕵️</div>
    <div class="course-code">BACS 3504</div>
    <div class="course-title">Security Incident Handling & Hacker Exploits</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('bacs3573')">
    <div class="course-icon">🐍</div>
    <div class="course-code">BACS 3573</div>
    <div class="course-title">Automating Information Security with Python</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('bacs4503')">
    <div class="course-icon">🔍</div>
    <div class="course-code">BACS 4503</div>
    <div class="course-title">Intrusion Detection In-Depth</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('bacs4499')">
    <div class="course-icon">🌐</div>
    <div class="course-code">BACS 4499</div>
    <div class="course-title">Internet Storm Center (ISC) Internship</div>
    <div class="course-status">Not Started</div>
  </div>
</div>

## Specialization Block (Months 13-24)

<div class="course-grid">
  <div class="course-card" onclick="openCourseModal('acs4560')">
    <div class="course-icon">🎯</div>
    <div class="course-code">ACS 4560</div>
    <div class="course-title">Network Penetration Testing & Ethical Hacking</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('acs4542')">
    <div class="course-icon">🌐</div>
    <div class="course-code">ACS 4542</div>
    <div class="course-title">Web App Penetration Testing & Ethical Hacking</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('acs4540')">
    <div class="course-icon">☁️</div>
    <div class="course-code">ACS 4540</div>
    <div class="course-title">Cloud Security and DevOps Automation</div>
    <div class="course-status">Not Started</div>
  </div>
</div>

---

<div class="phase-header">
🎓 MASTER'S PHASE (Months 25-60)
</div>

## Block 1: Foundation (Months 25-33)

<div class="course-grid">
  <div class="course-card" onclick="openCourseModal('ise5101')">
    <div class="course-icon">🏢</div>
    <div class="course-code">ISE 5101</div>
    <div class="course-title">Enterprise Information Security</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('ise5201')">
    <div class="course-icon">⚔️</div>
    <div class="course-code">ISE 5201</div>
    <div class="course-title">Hacking Techniques & Incident Response</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('ise5601')">
    <div class="course-icon">👔</div>
    <div class="course-code">ISE 5601</div>
    <div class="course-title">IT Security Leadership Competencies</div>
    <div class="course-status">Not Started</div>
  </div>
</div>

## Block 2: Organizational Application (Months 34-41)

<div class="course-grid">
  <div class="course-card" onclick="openCourseModal('ise6255')">
    <div class="course-icon">🏗️</div>
    <div class="course-code">ISE 6255</div>
    <div class="course-title">Defensible Security Architecture & Engineering</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('ise5401')">
    <div class="course-icon">🛡️</div>
    <div class="course-code">ISE 5401</div>
    <div class="course-title">Advanced Network Intrusion Detection & Analysis</div>
    <div class="course-status">Not Started</div>
  </div>
</div>

## Block 3: Specialization (Months 42-53)

<div class="course-grid">
  <div class="course-card" onclick="openCourseModal('ise6320')">
    <div class="course-icon">🎯</div>
    <div class="course-code">ISE 6320</div>
    <div class="course-title">Network Penetration Testing & Ethical Hacking</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('ise6315')">
    <div class="course-icon">🌐</div>
    <div class="course-code">ISE 6315</div>
    <div class="course-title">Web App Penetration Testing & Ethical Hacking</div>
    <div class="course-status">Not Started</div>
  </div>

  <div class="course-card" onclick="openCourseModal('ise6650')">
    <div class="course-icon">☁️</div>
    <div class="course-code">ISE 6650</div>
    <div class="course-title">Cloud Security and DevOps Automation</div>
    <div class="course-status">Not Started</div>
  </div>
</div>

## Block 4: Capstone (Months 54-60)

<div class="course-grid">
  <div class="course-card" onclick="openCourseModal('ise5901')">
    <div class="course-icon">📚</div>
    <div class="course-code">ISE 5901</div>
    <div class="course-title">Advanced Technical Research & Communication</div>
    <div class="course-status">Not Started</div>
  </div>
</div>

<!-- Course Modal -->
<div id="courseModal" class="modal">
  <div class="modal-content">
    <span class="close" onclick="closeModal()">&times;</span>
    <h2 id="modalTitle">Course Title</h2>
    <div id="modalContent">Course content will load here...</div>
    <h3>📝 My Notes</h3>
    <textarea id="courseNotes" class="notes-area" placeholder="Add your notes, insights, and progress here..."></textarea>
    <div>
      <button class="save-btn" onclick="saveNotes()">💾 Save Notes</button>
      <button class="save-btn" onclick="exportNotes()">📥 Export Notes</button>
    </div>
  </div>
</div>

<script>
const courseData = {
  'bacs3275': {
    title: 'BACS 3275: Foundations - Computers, Technology & Security',
    duration: '2 months', credits: 6,
    textbooks: ['CompTIA Security+ Study Guide (7th Edition)', 'Computer Networks (5th Edition)', 'Introduction to Programming Using Python (3rd Edition)'],
    labs: ['TryHackMe: Linux Fundamentals', 'HackTheBox Academy: Networking', 'Python security scripting'],
    objectives: ['Master computer architecture', 'Understand networking basics', 'Learn Python for security']
  },
  'bacs3301': { title: 'BACS 3301: Introduction to Cybersecurity', duration: '1 month', credits: 4, textbooks: ['Principles of Information Security (6th Edition)'], labs: ['Security awareness training', 'Basic firewall configuration'], objectives: ['Core security principles', 'Risk management', 'Security awareness'] },
  'bacs3402': { title: 'BACS 3402: Effective Cyber Writing and Speaking', duration: '1 month', credits: 3, textbooks: ['Technical Communication (12th Edition)'], labs: ['Security report writing', 'Presentation development'], objectives: ['Technical writing skills', 'Presentation abilities', 'Security communication'] },
  'bacs3401': { title: 'BACS 3401: Security Essentials', duration: '2 months', credits: 6, textbooks: ['Computer Security: Principles and Practice', 'Network Security Essentials'], labs: ['Network security monitoring', 'Endpoint protection'], objectives: ['Defense-in-depth strategies', 'Network security', 'Cloud security basics'] },
  'bacs3504': { title: 'BACS 3504: Security Incident Handling & Hacker Exploits', duration: '2 months', credits: 6, textbooks: ['The Hacker Playbook 3', 'Incident Response & Computer Forensics'], labs: ['Jr. Penetration Tester Path', 'Incident response scenarios'], objectives: ['Incident response procedures', 'Attacker methodologies', 'Digital forensics'] },
  'bacs3573': { title: 'BACS 3573: Automating Information Security with Python', duration: '1 month', credits: 4, textbooks: ['Automate the Boring Stuff with Python', 'Black Hat Python'], labs: ['Network reconnaissance tools', 'Log analysis scripts'], objectives: ['Python for security automation', 'Custom security tools', 'Automated workflows'] },
  'bacs4503': { title: 'BACS 4503: Intrusion Detection In-Depth', duration: '2 months', credits: 6, textbooks: ['Applied Network Security Monitoring', 'The Practice of Network Security Monitoring'], labs: ['Security Onion deployment', 'Suricata configuration'], objectives: ['Network security monitoring', 'Traffic analysis', 'IDS/IPS systems'] },
  'bacs4499': { title: 'BACS 4499: Internet Storm Center Internship', duration: '5 months', credits: 6, textbooks: ['Real-world threat analysis'], labs: ['Global threat monitoring', 'Attack pattern analysis'], objectives: ['Real-world experience', 'Threat analysis skills', 'Professional network'] },
  'acs4560': { title: 'ACS 4560: Network Penetration Testing & Ethical Hacking', duration: '3 months', credits: 3, textbooks: ['Penetration Testing: A Hands-On Introduction', 'Advanced Penetration Testing'], labs: ['HackTheBox machines', 'OSCP preparation'], objectives: ['Network penetration testing', 'Post-exploitation', 'OSCP preparation'] },
  'acs4542': { title: 'ACS 4542: Web App Penetration Testing & Ethical Hacking', duration: '3 months', credits: 3, textbooks: ['The Web Application Hacker\'s Handbook', 'Real-World Bug Hunting'], labs: ['OWASP WebGoat', 'Bug bounty practice'], objectives: ['Web application security', 'OWASP Top 10', 'API security'] },
  'acs4540': { title: 'ACS 4540: Cloud Security and DevOps Automation', duration: '3 months', credits: 3, textbooks: ['Cloud Security and Privacy', 'Securing DevOps'], labs: ['AWS/Azure security', 'CloudGoat scenarios'], objectives: ['Cloud security concepts', 'DevSecOps practices', 'Container security'] },
  'ise5101': { title: 'ISE 5101: Enterprise Information Security', duration: '3 months', credits: 3, textbooks: ['Computer Security: Principles and Practice', 'Network Security Essentials'], labs: ['Enterprise security architecture', 'Risk assessment frameworks'], objectives: ['Enterprise security design', 'Risk management', 'Compliance requirements'] },
  'ise5201': { title: 'ISE 5201: Hacking Techniques & Incident Response', duration: '3 months', credits: 3, textbooks: ['The Hacker Playbook 3', 'Incident Response & Computer Forensics'], labs: ['Advanced penetration testing', 'Complex incident response'], objectives: ['Advanced attack techniques', 'Lead incident response', 'Threat hunting'] },
  'ise5601': { title: 'ISE 5601: IT Security Leadership Competencies', duration: '3 months', credits: 3, textbooks: ['Information Security Governance Simplified', 'CISSP Official Study Guide'], labs: ['Security program development', 'Risk management planning'], objectives: ['Security leadership', 'Governance frameworks', 'Strategic risk management'] },
  'ise6255': { title: 'ISE 6255: Defensible Security Architecture & Engineering', duration: '3 months', credits: 3, textbooks: ['Building Secure and Reliable Systems', 'Security Architecture and Design'], labs: ['Zero-trust architecture', 'Security architecture assessments'], objectives: ['Secure system architectures', 'Zero-trust principles', 'Cloud security solutions'] },
  'ise5401': { title: 'ISE 5401: Advanced Network Intrusion Detection & Analysis', duration: '3 months', credits: 3, textbooks: ['Applied Network Security Monitoring', 'The Practice of Network Security Monitoring'], labs: ['Advanced SIEM deployment', 'Custom detection rules'], objectives: ['Advanced detection systems', 'Security analytics', 'Threat intelligence'] },
  'ise6320': { title: 'ISE 6320: Network Penetration Testing & Ethical Hacking', duration: '4 months', credits: 3, textbooks: ['Advanced Penetration Testing', 'Red Team Development and Operations'], labs: ['Enterprise penetration testing', 'Red team exercises'], objectives: ['Lead penetration testing', 'Red team operations', 'Advanced persistent threats'] },
  'ise6315': { title: 'ISE 6315: Web App Penetration Testing & Ethical Hacking', duration: '4 months', credits: 3, textbooks: ['The Web Application Hacker\'s Handbook', 'Real-World Bug Hunting'], labs: ['Advanced web app testing', 'API security assessments'], objectives: ['Advanced web app testing', 'Modern web architectures', 'Web security assessments'] },
  'ise6650': { title: 'ISE 6650: Cloud Security and DevOps Automation', duration: '4 months', credits: 3, textbooks: ['Securing DevOps', 'Container Security', 'Terraform: Up & Running'], labs: ['Multi-cloud security', 'Advanced container security'], objectives: ['Multi-cloud security', 'Containerized workloads', 'DevSecOps at scale'] },
  'ise5901': { title: 'ISE 5901: Advanced Technical Research & Communication', duration: '5 months', credits: 3, textbooks: ['The Craft of Research', 'Style: Lessons in Clarity and Grace'], labs: ['Original cybersecurity research', 'Academic paper writing'], objectives: ['Conduct original research', 'Publish academic papers', 'Present at conferences'] }
};

let courseNotes = {};

function openCourseModal(courseId) {
  const course = courseData[courseId];
  const modal = document.getElementById('courseModal');
  document.getElementById('modalTitle').textContent = course.title;
  document.getElementById('modalContent').innerHTML = `
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 20px 0;">
      <div><h4>📚 Course Details</h4><p><strong>Duration:</strong> ${course.duration}</p><p><strong>Credits:</strong> ${course.credits}</p></div>
      <div><h4>📖 Textbooks</h4><ul>${course.textbooks.map(book => `<li>${book}</li>`).join('')}</ul></div>
      <div><h4>🧪 Labs & Practice</h4><ul>${course.labs.map(lab => `<li>${lab}</li>`).join('')}</ul></div>
      <div><h4>🎯 Learning Objectives</h4><ul>${course.objectives.map(obj => `<li>${obj}</li>`).join('')}</ul></div>
    </div>
  `;
  document.getElementById('courseNotes').value = courseNotes[courseId] || '';
  modal.dataset.courseId = courseId;
  modal.style.display = 'block';
}

function closeModal() { document.getElementById('courseModal').style.display = 'none'; }

function saveNotes() {
  const modal = document.getElementById('courseModal');
  const courseId = modal.dataset.courseId;
  courseNotes[courseId] = document.getElementById('courseNotes').value;
  localStorage.setItem('courseNotes', JSON.stringify(courseNotes));
  alert('Notes saved! 💾');
}

function exportNotes() {
  const modal = document.getElementById('courseModal');
  const courseId = modal.dataset.courseId;
  const course = courseData[courseId];
  const notes = document.getElementById('courseNotes').value;
  const exportData = `# ${course.title}\n\n## My Notes\n${notes}\n\n## Course Info\n- Duration: ${course.duration}\n- Credits: ${course.credits}\n\nExported: ${new Date().toLocaleDateString()}`;
  const blob = new Blob([exportData], { type: 'text/markdown' });
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url; a.download = `${courseId}_notes.md`; a.click();
  URL.revokeObjectURL(url);
}

document.addEventListener('DOMContentLoaded', function() {
  const saved = localStorage.getItem('courseNotes');
  if (saved) courseNotes = JSON.parse(saved);
});

window.onclick = function(event) {
  const modal = document.getElementById('courseModal');
  if (event.target === modal) closeModal();
}
</script>
