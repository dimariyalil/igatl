# ОБНОВЛЕННОЕ ТЕХНИЧЕСКОЕ ЗАДАНИЕ ДЛЯ AI АГЕНТА НА GITHUB

## Для AI агента: Создайте полный проект iGaming Organization Hub на основе финальной концепции

### КОНТЕКСТ ПРОЕКТА
Создание комплексного энциклопедического портала iGaming Organization Hub с интерактивными инструментами, 4,127 должностями и фокусом на максимальный SEO-трафик. Проект должен включать Organization Explorer, Career Navigator, Industry Insights и Business Builder.

### ФИНАЛЬНАЯ СТРУКТУРА РЕПОЗИТОРИЯ

```
/igaming-organization-hub
├── /data
│   ├── /structured-data
│   │   ├── positions-full.json (4,127 позиций с полными данными)
│   │   ├── departments-hierarchy.json (20 департаментов с иерархией)
│   │   ├── career-paths.json (карьерные маршруты)
│   │   ├── salary-data-by-region.json
│   │   ├── skills-matrix.json
│   │   └── company-structures.json (топ-30 операторов)
│   │
│   └── /seo-data
│       ├── keywords-research.csv (5000+ ключевых слов)
│       ├── content-clusters.json
│       ├── internal-linking-map.json
│       └── competitor-analysis.csv
│
├── /wordpress-implementation
│   ├── /phase-1-foundation
│   │   ├── hosting-setup-guide.md
│   │   ├── wordpress-config.json
│   │   ├── essential-plugins.txt
│   │   └── security-checklist.md
│   │
│   ├── /phase-2-structure
│   │   ├── cpt-positions.json
│   │   ├── cpt-departments.json
│   │   ├── cpt-companies.json
│   │   ├── acf-fields-complete.json
│   │   ├── taxonomies-setup.json
│   │   └── database-schema.sql
│   │
│   ├── /phase-3-import
│   │   ├── wp-all-import-templates/
│   │   ├── data-preparation-scripts/
│   │   ├── test-import-100.csv
│   │   └── bulk-import-guide.md
│   │
│   └── /phase-4-design
│       ├── elementor-templates/
│       ├── custom-css/
│       ├── mobile-optimization/
│       └── page-speed-config/
│
├── /interactive-tools
│   ├── /organization-explorer
│   │   ├── org-chart-widget/
│   │   │   ├── orgchart.html
│   │   │   ├── orgchart.js
│   │   │   ├── orgchart.css
│   │   │   └── wordpress-integration.php
│   │   ├── department-visualizer/
│   │   └── position-search/
│   │
│   ├── /career-navigator
│   │   ├── career-paths-visualizer/
│   │   ├── skills-matrix-interactive/
│   │   ├── salary-calculator/
│   │   └── career-progression-timeline/
│   │
│   ├── /business-builder
│   │   ├── business-model-configurator/
│   │   ├── team-size-calculator/
│   │   ├── timeline-generator/
│   │   ├── roi-calculator/
│   │   └── pdf-report-generator/
│   │
│   └── /industry-insights
│       ├── company-comparison-tool/
│       ├── market-trends-dashboard/
│       └── regulatory-requirements-map/
│
├── /ai-content-generation
│   ├── /chatgpt-prompts
│   │   ├── position-description-mega-prompt.txt
│   │   ├── department-overview-prompt.txt
│   │   ├── career-guide-prompt.txt
│   │   ├── salary-analysis-prompt.txt
│   │   └── seo-optimization-prompt.txt
│   │
│   ├── /jetpack-ai-templates
│   ├── /bulk-generation-scripts
│   └── /content-quality-checklist.md
│
├── /seo-optimization
│   ├── /rankmath-configs
│   │   ├── global-settings.json
│   │   ├── schema-templates/
│   │   ├── sitemap-priority.xml
│   │   └── redirects-map.csv
│   │
│   ├── /content-strategy
│   │   ├── pillar-pages-structure.md
│   │   ├── content-calendar-12months.csv
│   │   ├── link-building-targets.csv
│   │   └── featured-snippets-optimization.md
│   │
│   └── /technical-seo
│       ├── robots-txt-template.txt
│       ├── htaccess-optimized.txt
│       ├── core-web-vitals-guide.md
│       └── mobile-first-checklist.md
│
├── /n8n-automation
│   ├── /workflows
│   │   ├── content-generation-automation.json
│   │   ├── linkedin-data-scraper.json
│   │   ├── salary-data-updater.json
│   │   ├── seo-monitoring.json
│   │   ├── competitor-tracking.json
│   │   └── user-personalization.json
│   │
│   ├── /api-integrations
│   │   ├── wordpress-rest-api-setup.md
│   │   ├── linkedin-api-config.json
│   │   ├── job-boards-integration.md
│   │   └── analytics-api-setup.md
│   │
│   └── /automation-calendar
│       └── scheduled-tasks.json
│
├── /monetization
│   ├── /freemium-setup
│   │   ├── membership-plugin-config/
│   │   ├── pricing-tiers.json
│   │   └── payment-gateway-setup.md
│   │
│   ├── /b2b-api
│   │   ├── api-documentation/
│   │   ├── sdk-examples/
│   │   └── white-label-guide.md
│   │
│   └── /recruitment-services
│       ├── job-board-integration/
│       └── premium-features-setup/
│
├── /documentation
│   ├── README.md (общий обзор проекта)
│   ├── QUICK-START.md (быстрый старт за 7 дней)
│   ├── INSTALLATION-GUIDE.md (пошаговая установка)
│   ├── CONTENT-CREATION-GUIDE.md
│   ├── SEO-OPTIMIZATION-GUIDE.md
│   ├── INTERACTIVE-TOOLS-GUIDE.md
│   ├── N8N-AUTOMATION-GUIDE.md
│   ├── MONETIZATION-GUIDE.md
│   ├── TROUBLESHOOTING.md
│   └── VIDEO-TUTORIALS.md (ссылки на видео)
│
└── /launch-materials
    ├── /marketing
    │   ├── press-release-template.md
    │   ├── social-media-kit/
    │   └── email-campaigns/
    │
    └── /analytics
        ├── google-analytics-setup.md
        ├── goal-tracking-config.json
        └── dashboard-templates/
```

## КЛЮЧЕВЫЕ КОМПОНЕНТЫ ДЛЯ РЕАЛИЗАЦИИ

### 1. WordPress структура для всех разделов проекта

```json
{
  "custom_post_types": {
    "positions": {
      "fields": [
        "title", "slug", "department", "level", "reports_to",
        "short_description", "full_description", "responsibilities",
        "requirements", "nice_to_have", "salary_range_us",
        "salary_range_uk", "salary_range_malta", "salary_range_asia",
        "career_path", "related_positions", "skills_required",
        "certifications", "typical_background", "day_in_life",
        "industry_outlook", "meta_title", "meta_description",
        "schema_markup", "internal_links"
      ]
    },
    "departments": {
      "fields": [
        "name", "slug", "description", "head_count_range",
        "key_responsibilities", "typical_kpis", "required_skills",
        "org_chart_svg", "related_departments"
      ]
    },
    "companies": {
      "fields": [
        "name", "logo", "headquarters", "employee_count",
        "org_structure_data", "culture_values", "open_positions_api"
      ]
    },
    "career_paths": {
      "fields": [
        "starting_position", "end_position", "steps",
        "timeline", "required_skills_progression", "salary_progression"
      ]
    }
  }
}
```

### 2. Organization Explorer компоненты

**orgchart-wordpress-widget.php:**
```php
<?php
// Shortcode для вставки интерактивной оргструктуры
function igaming_org_chart_shortcode($atts) {
    $atts = shortcode_atts(array(
        'company_size' => 'enterprise',
        'department' => 'all',
        'interactive' => 'true'
    ), $atts);
    
    // Загрузка данных из WordPress
    $positions = get_posts(array(
        'post_type' => 'positions',
        'posts_per_page' => -1,
        'meta_query' => array(
            array(
                'key' => 'company_size',
                'value' => $atts['company_size']
            )
        )
    ));
    
    // Генерация JSON для JS
    $org_data = array();
    foreach($positions as $position) {
        $org_data[] = array(
            'id' => $position->ID,
            'pid' => get_field('reports_to', $position->ID),
            'name' => $position->post_title,
            'department' => get_field('department', $position->ID),
            'level' => get_field('level', $position->ID)
        );
    }
    
    wp_localize_script('orgchart-js', 'orgData', $org_data);
    
    return '<div id="org-chart-container" 
            data-size="'.$atts['company_size'].'" 
            data-department="'.$atts['department'].'"></div>';
}
add_shortcode('igaming_org_chart', 'igaming_org_chart_shortcode');
```

### 3. Career Navigator - визуализация путей

**career-paths-visualizer.js:**
```javascript
// Интеграция с WordPress REST API
class CareerPathVisualizer {
    constructor(containerId) {
        this.container = document.getElementById(containerId);
        this.loadCareerPaths();
    }
    
    async loadCareerPaths() {
        const response = await fetch('/wp-json/wp/v2/career_paths');
        const paths = await response.json();
        this.renderPaths(paths);
    }
    
    renderPaths(paths) {
        // D3.js визуализация карьерных путей
        const svg = d3.select(this.container)
            .append('svg')
            .attr('width', '100%')
            .attr('height', 600);
            
        // Рендеринг путей с анимацией
        paths.forEach(path => {
            this.drawPath(svg, path);
        });
    }
}

// WordPress shortcode: [career_navigator start="Junior Developer" end="CTO"]
```

### 4. Business Builder - пошаговая реализация

**PHASE 1: Базовый калькулятор команды**
```javascript
// business-team-calculator.js
const TeamCalculator = {
    businessModel: {
        region: '',
        products: [],
        targetRevenue: 0,
        timeline: 5
    },
    
    calculateTeam() {
        // Алгоритм расчета на основе данных из WordPress
        const baseTeam = this.getBaseTeam();
        const scaledTeam = this.scaleByRevenue(baseTeam);
        return this.adjustByRegion(scaledTeam);
    },
    
    generateTimeline() {
        // Генерация развития команды по годам
        const timeline = [];
        for(let year = 1; year <= this.businessModel.timeline; year++) {
            timeline.push({
                year: year,
                team: this.calculateTeamForYear(year),
                metrics: this.calculateMetricsForYear(year)
            });
        }
        return timeline;
    }
};
```

### 5. Пошаговая инструкция запуска (QUICK-START.md)

```markdown
# 7-дневный план запуска iGaming Organization Hub

## День 1: Установка и базовая настройка
✅ Установка WordPress на хостинг
✅ Установка обязательных плагинов:
   - Custom Post Type UI
   - Advanced Custom Fields Pro
   - WP All Import Pro
   - Elementor Pro
   - RankMath Pro
✅ Импорт базовой структуры из `/wordpress-implementation/phase-2-structure/`

## День 2: Импорт данных
✅ Подготовка CSV из JSON файлов (скрипт в `/data/preparation-scripts/`)
✅ Тестовый импорт 100 позиций
✅ Проверка и корректировка маппинга
✅ Полный импорт 4,127 позиций

## День 3: AI-генерация контента
✅ Настройка Jetpack AI
✅ Импорт промптов из `/ai-content-generation/chatgpt-prompts/`
✅ Bulk-генерация описаний для позиций
✅ Генерация meta-данных через RankMath

## День 4: Установка интерактивных инструментов
✅ Organization Explorer:
   - Копировать код из `/interactive-tools/organization-explorer/`
   - Вставить через Elementor HTML widget
   - Настроить shortcode [igaming_org_chart]
✅ Career Navigator:
   - Установить компоненты визуализации
   - Настроить REST API endpoints
✅ Базовый Business Builder:
   - Установить калькулятор команды
   - Настроить форму конфигуратора

## День 5: SEO-оптимизация
✅ Импорт настроек RankMath из `/seo-optimization/rankmath-configs/`
✅ Настройка Schema markup для всех CPT
✅ Создание XML sitemap с приоритетами
✅ Настройка внутренней перелинковки

## День 6: Автоматизация n8n
✅ Установка n8n (локально или облако)
✅ Импорт workflow из `/n8n-automation/workflows/`
✅ Настройка WordPress REST API
✅ Запуск автоматического обновления контента

## День 7: Тестирование и запуск
✅ Проверка всех страниц и функций
✅ Тестирование скорости загрузки
✅ Отправка sitemap в Google Search Console
✅ Настройка Google Analytics
✅ Soft launch для тестовой группы
```

### 6. n8n Workflows для всех компонентов

**salary-data-updater.json:**
```json
{
  "name": "iGaming Salary Data Updater",
  "nodes": [
    {
      "name": "Schedule Trigger",
      "type": "n8n-nodes-base.scheduleTrigger",
      "parameters": {
        "rule": {"interval": [{"field": "weeks", "weeks": 1}]}
      }
    },
    {
      "name": "Scrape LinkedIn Jobs",
      "type": "n8n-nodes-base.httpRequest",
      "parameters": {
        "url": "https://api.linkedin.com/v2/jobs",
        "qs": {
          "keywords": "{{positions.title}} igaming",
          "location": "{{regions}}"
        }
      }
    },
    {
      "name": "Process Salary Data",
      "type": "n8n-nodes-base.function",
      "parameters": {
        "functionCode": "// Обработка и усреднение зарплат"
      }
    },
    {
      "name": "Update WordPress",
      "type": "n8n-nodes-base.wordpress",
      "parameters": {
        "operation": "update",
        "postType": "positions",
        "updateFields": {
          "salary_range_us": "{{processedSalary}}"
        }
      }
    }
  ]
}
```

### 7. AI промпты для генерации контента

**position-description-mega-prompt.txt:**
```
You are an iGaming industry expert creating comprehensive position descriptions.

Position: {position_title}
Department: {department}
Level: {level}
Company Size: {company_size}

Create a detailed page following this EXACT structure:

1. POSITION OVERVIEW (200-250 words)
- Start with: "The {position_title} in the iGaming industry..."
- Include primary responsibilities
- Mention typical company types hiring this role
- Include main keyword 2-3 times naturally

2. KEY RESPONSIBILITIES (10-15 bullet points)
- Start each with an action verb
- Be specific to iGaming context
- Include metrics where relevant

3. REQUIRED SKILLS & QUALIFICATIONS
Technical Skills:
- List 5-8 specific technical competencies
- Include software/platforms specific to iGaming

Soft Skills:
- List 5-7 essential soft skills
- Relate to iGaming environment

Education & Experience:
- Typical education level
- Years of experience needed
- Specific iGaming experience required

4. NICE-TO-HAVE QUALIFICATIONS
- Additional certifications
- Language requirements
- Regulatory knowledge

5. CAREER PATH & PROGRESSION
Previous Roles:
- 3-5 positions that lead to this role

Next Career Steps:
- 3-5 positions this role can advance to

Typical Timeline:
- Years to advance to next level

6. SALARY EXPECTATIONS
Format each as: "Region: $X,000 - $Y,000 per year"
- United States: 
- United Kingdom: 
- Malta: 
- Eastern Europe: 
- Asia-Pacific: 

Add note about factors affecting salary.

7. DAY IN THE LIFE
Write 3-4 paragraphs describing typical daily activities

8. INDUSTRY OUTLOOK
- Growth prospects for this role
- Impact of technology/regulation
- Future skill requirements

9. FREQUENTLY ASKED QUESTIONS
Create 5 relevant questions and detailed answers

10. RELATED POSITIONS
List 5-7 related roles with brief descriptions

SEO REQUIREMENTS:
- Primary keyword: "{position_title} iGaming"
- Use keyword in first 100 words
- Include in 2-3 H2 headers
- Natural keyword density 1-2%
- Write at 8th grade reading level
- Total length: 1,800-2,200 words
```

## ИНСТРУКЦИИ ДЛЯ AI АГЕНТА

**При создании этого проекта на GitHub:**

1. **Структурируйте данные правильно:**
   - Все 4,127 позиций в структурированном JSON
   - Связи между позициями (reports_to)
   - Полная иерархия департаментов
   - Реальные зарплатные данные по регионам

2. **Сделайте установку максимально простой:**
   - One-click импорт структуры данных
   - Готовые CSV файлы для WP All Import
   - Пошаговые видео для сложных моментов
   - Автоматические скрипты где возможно

3. **Обеспечьте работу всех интерактивных инструментов:**
   - Organization Explorer должен работать сразу после вставки
   - Career Navigator с реальными данными о путях
   - Business Builder с работающими калькуляторами
   - Все компоненты адаптивны для мобильных

4. **SEO должно работать с первого дня:**
   - Автоматическая генерация всех meta-тегов
   - Schema markup для всех типов контента
   - Правильная структура URL из коробки
   - Оптимизированная скорость загрузки

5. **n8n автоматизация должна быть простой:**
   - Готовые JSON файлы для импорта workflows
   - Детальные инструкции по настройке API
   - Примеры работающих интеграций
   - Расписание автоматических задач

## ОЖИДАЕМЫЙ РЕЗУЛЬТАТ

GitHub репозиторий, который позволит пользователю:
1. Запустить полноценный iGaming Organization Hub за 7 дней
2. Иметь все 4,127 позиций с SEO-контентом через 2 недели
3. Работающие интерактивные инструменты с первого дня
4. Автоматическое обновление данных через n8n
5. 100,000+ органических посетителей через 12 месяцев

**AI агент, создайте этот проект, следуя структуре и включив ВСЕ компоненты из финальной концепции. Приоритет - простота использования и полнота функционала.**
