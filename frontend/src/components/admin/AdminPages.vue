<template>
    <div class="admin-pages">
        <PageTitle icon="fa fa-cogs" main="Administração do Sistema"
            sub="Cadastros & Cia" />
        <div class="admin-pages-tabs">
            <b-card no-body>
                <b-tabs card>
                    <b-tab title="Artigo">
                        <ArticleAdmin />
                    </b-tab>
                    <b-tab title="Categoria">
                        <CategoryAdmin />
                    </b-tab>
                    <b-tab title="Usuário" active>
                        <UserAdmin />
                    </b-tab>
                </b-tabs>
            </b-card>
        </div>
    </div>
</template>

<script>
import PageTitle from '@/components/template/PageTitle'
import ArticleAdmin from '@/components/admin/ArticleAdmin'
import CategoryAdmin from '@/components/admin/CategoryAdmin'
import UserAdmin from '@/components/admin/UserAdmin'
export default {
    name: 'AdminPages',
    components: { PageTitle, ArticleAdmin, CategoryAdmin, UserAdmin }
}
</script>

<style>

</style>
