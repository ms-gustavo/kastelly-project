<h1>🏬 Kastelly - Sistema de Gestão para Loja de Móveis Planejados</h1>

<p><strong>Kastelly</strong> é uma solução completa para a gestão de lojas de móveis planejados, composta por uma <strong>aplicação desktop</strong> desenvolvida em Electron + React e uma <strong>API REST</strong> robusta com Spring Boot + MongoDB.</p>

<hr />

<h2>📦 Aplicação Desktop (Frontend)</h2>

<h3>🛠 Tecnologias Utilizadas</h3>
<ul>
  <li>Electron – execução como app desktop</li>
  <li>React + Vite – construção da interface</li>
  <li>React Hook Form + Yup – validação e controle de formulários</li>
  <li>Zustand – gerenciamento de estado global</li>
  <li>Axios – requisições HTTP</li>
  <li>Tailwind CSS – estilização utilitária</li>
</ul>

<h3>📁 Estrutura de Pastas</h3>
<pre style="background: #f6f8fa; padding: 1rem; border-radius: 6px;">
├── api/
├── assets/
├── components/
│   ├── budgets/
│   ├── clients/
│   └── contracts/
├── enums/
├── interfaces/
├── layouts/
├── pages/
│   ├── budgets/
│   ├── clients/
│   └── contracts/
├── schemas/
├── store/
└── main.tsx
</pre>

<h3>✅ Funcionalidades Implementadas</h3>
<ul>
  <li>Cadastro, edição, visualização e exclusão de <strong>Clientes</strong></li>
  <li>Criação e listagem de <strong>Orçamentos</strong> com totais</li>
  <li>Criação e listagem de <strong>Contratos</strong> com múltiplas descrições</li>
  <li>Geração de <strong>PDF</strong> (via backend)</li>
  <li>Envio de PDFs por e-mail (via backend)</li>
  <li>Interface intuitiva e responsiva</li>
  <li>Validações robustas nos formulários</li>
</ul>

<h3>📎 Observações</h3>
<ul>
  <li>Aplicação exclusiva para ambiente <strong>desktop</strong> (sem suporte a PWA)</li>
  <li>UI com <strong>Tailwind CSS puro</strong>, sem bibliotecas externas</li>
</ul>

<hr />

<h2>🔗 API Backend (Spring Boot)</h2>

<h3>🧩 Tecnologias Utilizadas</h3>
<ul>
  <li>Java 17+</li>
  <li>Spring Boot + Spring Data MongoDB</li>
  <li>MongoDB Atlas</li>
  <li>Lombok, Jakarta Bean Validation</li>
  <li>OpenHtmlToPdf – geração de PDFs</li>
  <li>JavaMailSender – envio de e-mails com anexo</li>
  <li>SpringDoc OpenAPI – documentação Swagger</li>
  <li>JUnit 5 + Mockito – testes automatizados</li>
</ul>

<h3>📁 Estrutura de Pastas</h3>
<ul>
  <li><code>entities</code> – Client, Contract, Budget, Address, MaterialItem</li>
  <li><code>dtos</code> – objetos de transferência de dados</li>
  <li><code>repositories</code> – acesso ao MongoDB</li>
  <li><code>services</code> – lógica de negócio, PDF, e-mail</li>
  <li><code>controllers</code> – endpoints REST</li>
  <li><code>interfaces</code> – contratos de serviços</li>
  <li><code>exceptions</code> – tratativas globais de erro</li>
  <li><code>builders</code> – construção de arquivos e componentes</li>
  <li><code>utils</code> – utilitários auxiliares</li>
  <li><code>config</code> – configurações do projeto</li>
</ul>

<h3>📌 Funcionalidades Backend</h3>
<ul>
  <li>CRUD de <strong>Clientes</strong>, <strong>Orçamentos</strong> e <strong>Contratos</strong></li>
  <li>Associação de contratos/orçamentos aos clientes</li>
  <li>Geração de <strong>PDFs personalizados</strong> com HTML e CSS</li>
  <li>Envio automatizado de e-mails com PDFs</li>
  <li>Armazenamento local dos arquivos em <code>Desktop/Clientes/{cliente}/{ano}</code></li>
  <li>Tratamento global de erros com mensagens padronizadas</li>
  <li>Documentação via Swagger (<a href="http://localhost:8080/swagger-ui.html" target="_blank">/swagger-ui.html</a>)</li>
</ul>

<h3>📄 Geração de PDFs</h3>
<ul>
  <li>Templates HTML para <strong>contrato</strong> e <strong>orçamento</strong></li>
  <li>Suporte a tabelas dinâmicas e imagens (como logotipo)</li>
  <li>Conversão de valores monetários para o formato brasileiro</li>
</ul>

<h3>📧 Envio de E-mails</h3>
<ul>
  <li>PDF enviado como anexo com corpo personalizado</li>
  <li>Validação de e-mail, erros de envio e arquivos ausentes</li>
</ul>

<h3>🧪 Testes Automatizados</h3>
<ul>
  <li>100% dos serviços testados com <strong>JUnit 5 + Mockito</strong></li>
  <li>Testes de controllers com <strong>MockMvc</strong></li>
  <li>Mocks estáticos com <code>mockito-inline</code></li>
</ul>

<h3>🔗 Endpoints Principais</h3>
<ul>
  <li><code>GET /api/clients</code> – Listar clientes</li>
  <li><code>POST /api/contracts</code> – Criar contrato</li>
  <li><code>POST /api/budgets</code> – Criar orçamento</li>
  <li><code>GET /api/pdfs/{id}?type=CONTRACT</code> – Gerar PDF</li>
  <li><code>GET /api/pdfs/{id}/send?type=BUDGET</code> – Enviar PDF por e-mail</li>
</ul>

<hr />

<h2>📈 Planejamento Futuro</h2>
<ul>
  <li>CRUD de Projetos</li>
  <li>Módulo de Finanças</li>
  <li>Histórico de alterações</li>
  <li>Visualização e upload de PDFs no frontend</li>
  <li>Autenticação com JWT</li>
  <li>Integração com AWS S3</li>
  <li>Logs no ELK Stack</li>
  <li>Notificações e interações offline</li>
</ul>

<hr />

<p><strong>Para dúvidas, melhorias ou contribuições, entre em contato comigo.</strong></p>
