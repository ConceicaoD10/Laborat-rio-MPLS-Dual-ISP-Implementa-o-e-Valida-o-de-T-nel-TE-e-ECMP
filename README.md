# Laborat-rio-MPLS-Dual-ISP-Implementa-o-e-Valida-o-de-T-nel-TE-e-ECMP

Este laboratório simula uma infraestrutura MPLS multihomed com dois backbones (Vodafone e OBS), permitindo o estudo de VRFs, ECMP, túneis MPLS TE e redundância de tráfego para clientes corporativos. O objetivo é aplicar conceitos de engenharia de tráfego avançada em um ambiente controlado, refletindo cenários reais de provedores e grandes corporações.

Objetivos

Implementar VRFs por cliente com isolamento completo de rede e rotas.

Configurar MP-BGP VPNv4 entre roteadores PE para interconexão de VRFs.

Implementar MPLS Traffic Engineering (RSVP-TE) com túneis primários e secundários.

Ativar ECMP (Equal Cost Multi-Path) para balanceamento de tráfego entre backbones.

Organizar as configurações de forma clara para estudo e análise.


Tarefas Realizadas

1. Configuração de VRFs e Route-Targets

VRFs criadas para clientes como CIB-HQ, NPE-HQ e HSBC.

Definidos route-target import/export para controle de propagação de rotas.


2. Configuração do Underlay

OSPFv2/OSPFv3 entre PE e core.

MPLS TE habilitado nas interfaces core para suporte a RSVP-TE.

Definição de explicit-paths para caminhos primário e secundário.

3. Configuração de BGP e ECMP

MP-BGP VPNv4 configurado entre PE para interconexão de VRFs.

maximum-paths 2 configurado para ECMP, permitindo múltiplos next-hops.

4. Preparação de Túneis TE

Túneis MPLS TE (Tunnel100, Tunnel200) configurados com caminhos primário e secundário.

Bandwidth e prioridades ajustados para simular engenharia de tráfego em produção.

5. Organização das Configurações

Arquivos de configuração separados por roteador para facilitar análise e estudo.

Estrutura preparada para importação direta em EVE-NG ou versão prática em laboratório físico.

Significado na Infraestrutura Real

VRFs: Isolamento de tráfego para diferentes clientes, prática padrão em ISPs e grandes empresas.

MPLS TE: Engenharia de tráfego para evitar congestionamentos e garantir SLA.

ECMP: Redundância e balanceamento, aumentando resiliência da rede.

MP-BGP VPNv4: Base para serviços de VPN escaláveis e integração de múltiplos backbones.


O laboratório representa cenários reais de provedores e grandes corporações, como balanceamento entre múltiplos ISPs, redundância de tráfego e planejamento avançado de caminhos TE.


Relevância Técnica

Aplicação prática de conceitos avançados de MPLS, BGP, VRF, ECMP e TE.

Experiência com planejamento de redes multihomed, isolamento de clientes e redundância.

Preparação para implementação em ambientes corporativos e provedores de serviço de alta disponibilidade.
