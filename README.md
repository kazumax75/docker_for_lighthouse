Laravel��GraphQL���C�u����lighthouse�̃e�X�g�p�ɍ����docker���B
/src���Ɂularavel�v�t�H���_�Ƃ��ĉ��L���|�W�g��git pull���Ă����B

lighthouse-example
https://github.com/nuwave/lighthouse-example

lighthouse-tutorial
https://github.com/nuwave/lighthouse-tutorial


�E�e��o�[�W����
PHP8.0
Composer version 2.3.3
mysql5.7

DB�̃z�X�g���|�[�g��4306

�v���C�O���E���hURL
http://127.0.0.1:8001/graphql-playground

.env.laravel��.env�Ƀ��l�[������pull���laravel�v���W�F�N�g�ɒu���ǂ�


�}�C�O���[�V����
php artisan migrate


�t�@�N�g���[
php artisan tinker
\App\Models\Comment::factory(10)->create()


========================================================

�E���ӓ_�A�n�}�����
dc.yml��MYSQL_PASSWORD��MYSQL_ROOT_PASSWORD�ɓ����p�X���[�h������ƃG���[�ƂȂ�db�R���e�i���I�����Ă��܂��B
.env��DB���[�U��MYSQL_USER���w��Broot���[�U�w�肷��ƃ}�C�O���[�V�������s�����[�U����SQL�G���[���o��B

���܂ł�docker���ł͋��L��DB���g�p���Ă�������DB�R���e�i�֌W���T�������������̂Ń����O�O�G
