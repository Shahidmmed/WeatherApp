<script>
import { Link } from "svelte-routing";
</script>

        <nav class="uk-navbar-container uk-navbar-transparent" uk-navbar>
            <div class="uk-navbar-left">
                <ul class="uk-navbar-nav">
                    <li class="uk-active"><Link>Active</Link></li>
                    <li><Link>Item</Link></li>
                    <li>
                        <Link>Parent</Link>
                        <div class="uk-navbar-dropdown">
                            <ul class="uk-nav uk-navbar-dropdown-nav">
                                <li class="uk-active"><Link>Active</Link></li>
                                <li><Link>Item</Link></li>
                                <li class="uk-nav-header">Header</li>
                                <li><Link>Item</Link></li>
                                <li><Link>Item</Link></li>
                                <li class="uk-nav-divider"></li>
                                <li><Link>Item</Link></li>
                            </ul>
                        </div>
                    </li>
                </ul>
            </div>
        </nav>
