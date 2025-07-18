<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Haake Móveis - Marcenaria de Qualidade</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            scroll-behavior: smooth;
        }
        
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://placehold.co/1920x1080');
            background-size: cover;
            background-position: center;
        }
        
        .gallery-image {
            transition: transform 0.3s;
            cursor: pointer;
        }
        
        .gallery-image:hover {
            transform: scale(1.03);
        }
        
        .modal-image {
            max-width: 80vw;
            max-height: 80vh;
            transition: transform 0.3s;
        }
        
        .contact-form input, 
        .contact-form textarea {
            transition: border 0.3s;
        }
        
        .contact-form input:focus, 
        .contact-form textarea:focus {
            border-color: #8B5A2B;
            outline: none;
        }
        
        .zoom-in {
            transform: scale(1.1);
        }
    </style>
</head>
<body>
    <!-- Cabeçalho -->
    <header class="bg-amber-900 text-white shadow-lg">
        <div class="container mx-auto px-4 py-6 flex justify-between items-center">
            <div class="flex items-center">
                <h1 class="text-2xl md:text-3xl font-bold">HA<span class="text-amber-200">AKE</span> MÓVEIS</h1>
            </div>
            <nav>
                <ul class="flex space-x-6">
                    <li><a href="#inicio" class="hover:text-amber-200 transition">Início</a></li>
                    <li><a href="#servicos" class="hover:text-amber-200 transition">Serviços</a></li>
                    <li><a href="#portfolio" class="hover:text-amber-200 transition">Portfólio</a></li>
                    <li><a href="#contato" class="hover:text-amber-200 transition">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Seção Hero -->
    <section id="inicio" class="hero h-screen flex items-center">
        <div class="container mx-auto px-4 text-center text-white">
            <h2 class="text-4xl md:text-6xl font-bold mb-6">Móveis Sob Medida Com Excelência</h2>
            <p class="text-xl md:text-2xl mb-8">Transformamos sua visão em realidade com madeira de qualidade e design atemporal</p>
            <a href="#contato" class="bg-amber-700 hover:bg-amber-600 text-white px-8 py-3 rounded-lg font-bold transition">Solicite Orçamento</a>
        </div>
    </section>

    <!-- Seção Serviços -->
    <section id="servicos" class="py-20 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16 text-amber-900">Nossos Serviços</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-10">
                <div class="bg-white p-6 rounded-lg shadow-lg">
                    <div class="h-48 mb-4 overflow-hidden rounded">
                        <img src="https://placehold.co/600x400" alt="Projeto 3D de móvel planejado mostrando diferentes ângulos" class="w-full h-full object-cover" />
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-amber-800">Projeto 3D Personalizado</h3>
                    <p class="text-gray-600">Criamos renderizações 3D realistas para você visualizar seu móvel antes da produção.</p>
                </div>
                
                <div class="bg-white p-6 rounded-lg shadow-lg">
                    <div class="h-48 mb-4 overflow-hidden rounded">
                        <img src="https://placehold.co/600x400" alt="Marcenaria trabalhando com diferentes tipos de madeira nobre" class="w-full h-full object-cover" />
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-amber-800">Marcenaria Especializada</h3>
                    <p class="text-gray-600">Trabalhamos com madeiras nobres e técnicas tradicionais para móveis duráveis.</p>
                </div>
                
                <div class="bg-white p-6 rounded-lg shadow-lg">
                    <div class="h-48 mb-4 overflow-hidden rounded">
                        <img src="https://placehold.co/600x400" alt="Móveis prontos sendo instalados em residência" class="w-full h-full object-cover" />
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-amber-800">Instalação Profissional</h3>
                    <p class="text-gray-600">Entregamos e instalamos seus móveis com cuidado e atenção aos detalhes.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção Portfólio -->
    <section id="portfolio" class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16 text-amber-900">Conheça Nosso Trabalho</h2>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Item 1 -->
                <div class="overflow-hidden rounded-lg shadow-md hover:shadow-xl transition">
                    <div class="relative overflow-hidden h-60">
                        <img src="https://placehold.co/800x600" alt="Cozinha planejada em carvalho com ilha central e bancada em granito" class="gallery-image w-full h-full object-cover" data-target="modal1" />
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg text-amber-800">Cozinha Planejada</h3>
                        <p class="text-gray-600">Móveis em carvalho com acabamento envelhecido</p>
                    </div>
                </div>
                
                <!-- Item 2 -->
                <div class="overflow-hidden rounded-lg shadow-md hover:shadow-xl transition">
                    <div class="relative overflow-hidden h-60">
                        <img src="https://placehold.co/800x600" alt="Escritório executivo em madeira maciça com prateleiras embutidas" class="gallery-image w-full h-full object-cover" data-target="modal2" />
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg text-amber-800">Escritório Executivo</h3>
                        <p class="text-gray-600">Conjunto em peroba rosa com detalhes em latão</p>
                    </div>
                </div>
                
                <!-- Item 3 -->
                <div class="overflow-hidden rounded-lg shadow-md hover:shadow-xl transition">
                    <div class="relative overflow-hidden h-60">
                        <img src="https://placehold.co/800x600" alt="Estante modular para sala de estar com nichos e portas de vidro" class="gallery-image w-full h-full object-cover" data-target="modal3" />
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg text-amber-800">Estante Modular</h3>
                        <p class="text-gray-600">Design moderno com estrutura em eucalipto</p>
                    </div>
                </div>
                
                <!-- Item 4 -->
                <div class="overflow-hidden rounded-lg shadow-md hover:shadow-xl transition">
                    <div class="relative overflow-hidden h-60">
                        <img src="https://placehold.co/800x600" alt="Armário de quarto conjugado com espelho e gavetas embutidas" class="gallery-image w-full h-full object-cover" data-target="modal4" />
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg text-amber-800">Armário de Casal</h3>
                        <p class="text-gray-600">Compartimentos inteligentes e portas corrediças</p>
                    </div>
                </div>
                
                <!-- Item 5 -->
                <div class="overflow-hidden rounded-lg shadow-md hover:shadow-xl transition">
                    <div class="relative overflow-hidden h-60">
                        <img src="https://placehold.co/800x600" alt="Banheiro com mobília em teca com pia suspensa e armário" class="gallery-image w-full h-full object-cover" data-target="modal5" />
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg text-amber-800">Mobília de Banheiro</h3>
                        <p class="text-gray-600">Teca tratada para umidade com acabamento premium</p>
                    </div>
                </div>
                
                <!-- Item 6 -->
                <div class="overflow-hidden rounded-lg shadow-md hover:shadow-xl transition">
                    <div class="relative overflow-hidden h-60">
                        <img src="https://placehold.co/800x600" alt="Painel ilustrativo mostrando render 3D e comparação com produto final" class="gallery-image w-full h-full object-cover" data-target="modal6" />
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg text-amber-800">Projeto 3D vs Realidade</h3>
                        <p class="text-gray-600">Veja como nossos projetos se tornam realidade</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção Contato -->
    <section id="contato" class="py-20 bg-amber-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16 text-amber-900">Entre em Contato</h2>
            
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="text-2xl font-bold mb-6 text-amber-800">Fale Conosco</h3>
                    <p class="mb-8 text-gray-700">Estamos prontos para transformar suas ideias em móveis exclusivos. Preencha o formulário ou use nossos contatos diretos.</p>
                    
                    <div class="space-y-4">
                        <div class="flex items-start">
                            <div class="mr-4 mt-1 text-amber-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                                </svg>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Telefone</h4>
                                <p class="text-gray-600">(XX) XXXX-XXXX</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="mr-4 mt-1 text-amber-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                                </svg>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">E-mail</h4>
                                <p class="text-gray-600">contato@haake.moveis.com</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="mr-4 mt-1 text-amber-700">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                                </svg>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Endereço</h4>
                                <p class="text-gray-600">Av. das Oficinas, 123 - Bairro Industrial - Cidade/UF</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white p-8 rounded-lg shadow-lg">
                    <form class="contact-form">
                        <div class="mb-6">
                            <label for="nome" class="block text-gray-700 mb-2 font-medium">Nome Completo</label>
                            <input type="text" id="nome" class="w-full px-4 py-2 border rounded-lg focus:border-amber-500" required>
                        </div>
                        
                        <div class="mb-6">
                            <label for="email" class="block text-gray-700 mb-2 font-medium">E-mail</label>
                            <input type="email" id="email" class="w-full px-4 py-2 border rounded-lg focus:border-amber-500" required>
                        </div>
                        
                        <div class="mb-6">
                            <label for="telefone" class="block text-gray-700 mb-2 font-medium">Telefone</label>
                            <input type="tel" id="telefone" class="w-full px-4 py-2 border rounded-lg focus:border-amber-500" required>
                        </div>
                        
                        <div class="mb-6">
                            <label for="mensagem" class="block text-gray-700 mb-2 font-medium">Sua Mensagem</label>
                            <textarea id="mensagem" rows="5" class="w-full px-4 py-2 border rounded-lg focus:border-amber-500" required></textarea>
                        </div>
                        
                        <div class="flex items-center">
                            <button type="submit" class="bg-amber-700 hover:bg-amber-600 text-white px-6 py-3 rounded-lg font-bold transition">Enviar Mensagem</button>
                            <div class="ml-4 text-sm text-gray-600">
                                Responderemos em até 24 horas
                            </div>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Modal para imagens ampliadas -->
    <div id="imageModal" class="fixed inset-0 bg-black bg-opacity-75 z-50 hidden items-center justify-center">
        <div class="relative">
            <span id="closeModal" class="absolute -top-10 right-0 text-white text-3xl cursor-pointer">&times;</span>
            <img id="modalImage" class="modal-image" src="" alt="Imagem ampliada">
            <div class="flex justify-center mt-4 space-x-4">
                <button id="zoomIn" class="bg-white px-4 py-2 rounded">+ Zoom</button>
                <button id="zoomOut" class="bg-white px-4 py-2 rounded">- Zoom</button>
                <button id="resetZoom" class="bg-white px-4 py-2 rounded">Resetar</button>
            </div>
        </div>
    </div>

    <!-- Rodapé -->
    <footer class="bg-amber-900 text-white py-8">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <h2 class="text-2xl font-bold">HA<span class="text-amber-200">AKE</span> MÓVEIS</h2>
                    <p class="mt-2 text-amber-100">Marcenaria de qualidade desde 1995</p>
                </div>
                
                <div class="flex space-x-6">
                    <a href="#" class="text-amber-200 hover:text-white transition">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M22.675 0h-21.35c-.732 0-1.325.593-1.325 1.325v21.351c0 .731.593 1.324 1.325 1.324h11.495v-9.294h-3.128v-3.622h3.128v-2.671c0-3.1 1.893-4.788 4.659-4.788 1.325 0 2.463.099 2.795.143v3.24l-1.918.001c-1.504 0-1.795.715-1.795 1.763v2.313h3.587l-.467 3.622h-3.12v9.293h6.116c.73 0 1.323-.593 1.323-1.325v-21.35c0-.732-.593-1.325-1.325-1.325z"/>
                        </svg>
                    </a>
                    <a href="#" class="text-amber-200 hover:text-white transition">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
                        </svg>
                    </a>
                    <a href="#" class="text-amber-200 hover:text-white transition">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"/>
                        </svg>
                    </a>
                </div>
            </div>
            
            <div class="border-t border-amber-800 mt-8 pt-8 text-sm text-center text-amber-200">
                <p>&copy; 2023 Haake Móveis. Todos os direitos reservados.</p>
                <p class="mt-2">Projetos em 3D e móveis sob medida com qualidade premium.</p>
            </div>
        </div>
    </footer>

    <script>
        // Modal para imagens ampliadas
        document.addEventListener('DOMContentLoaded', function() {
            const galleryImages = document.querySelectorAll('.gallery-image');
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            const closeModal = document.getElementById('closeModal');
            const zoomInBtn = document.getElementById('zoomIn');
            const zoomOutBtn = document.getElementById('zoomOut');
            const resetZoomBtn = document.getElementById('resetZoom');
            
            let currentScale = 1;
            
            // Abrir modal ao clicar na imagem
            galleryImages.forEach(img => {
                img.addEventListener('click', function() {
                    modal.classList.remove('hidden');
                    modal.classList.add('flex');
                    modalImg.src = this.src;
                    modalImg.alt = this.alt;
                    modalImg.style.transform = 'scale(1)';
                    currentScale = 1;
                });
            });
            
            // Fechar modal
            closeModal.addEventListener('click', function() {
                modal.classList.add('hidden');
                modal.classList.remove('flex');
            });
            
            // Fechar modal clicando fora
            modal.addEventListener('click', function(e) {
                if (e.target === modal) {
                    modal.classList.add('hidden');
                    modal.classList.remove('flex');
                }
            });
            
            // Zoom functions
            zoomInBtn.addEventListener('click', function() {
                currentScale += 0.1;
                modalImg.style.transform = `scale(${currentScale})`;
            });
            
            zoomOutBtn.addEventListener('click', function() {
                if (currentScale > 0.2) {
                    currentScale -= 0.1;
                    modalImg.style.transform = `scale(${currentScale})`;
                }
            });
            
            resetZoomBtn.addEventListener('click', function() {
                currentScale = 1;
                modalImg.style.transform = 'scale(1)';
            });
            
            // Form submission (simulado)
            const contactForm = document.querySelector('.contact-form');
            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                alert('Mensagem enviada com sucesso! Entraremos em contato em breve.');
                this.reset();
            });
        });
    </script>
</body>
</html>
